![Libertad VZLA](/public/logo-500.png)

# Libertad VZLA: Plataforma de Noticias Full-Stack

[🇺🇸 English](README.md) | [🇵🇹 Português](README.pt.md)

<p align="center">
  <img src="https://img.shields.io/badge/Next.js-14+-black?style=for-the-badge&logo=next.js" alt="Next.js" />
  <img src="https://img.shields.io/badge/TypeScript-Strict-blue?style=for-the-badge&logo=typescript" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Supabase-Database-green?style=for-the-badge&logo=supabase" alt="Supabase" />
  <img src="https://img.shields.io/badge/TailwindCSS-Styling-06B6D4?style=for-the-badge&logo=tailwindcss" alt="Tailwind CSS" />
</p>

## 🏛️ Resumen del Proyecto

Este repositorio contiene el código fuente de un sistema de gestión de contenido y distribución de noticias de alto rendimiento. Construido con estándares web modernos, utiliza **Server-Side Rendering (SSR) de Next.js**, **Server Actions**, y un backend **PostgreSQL de Supabase**. La arquitectura está diseñada para priorizar la entrega rápida de contenido, la mantenibilidad y flujos de trabajo administrativos robustos.

---

## ⚙️ Características Técnicas Principales

### 1. Ingeniería de Rendimiento

Optimización sistemática de la latencia de red y ciclos de renderizado. La plataforma se adhiere a las métricas Core Web Vitals utilizando React Server Components (RSC) y streaming dinámico para minimizar los bundles de Javascript y mejorar el Time to First Byte (TTFB).

### 2. Integridad de Datos y Seguridad

Implementado con una arquitectura desacoplada utilizando una capa granular de validación de identidad. Aprovechamos Row-Level Security (RLS) de Supabase para aplicar políticas de acceso a datos directamente en la capa de base de datos, protegiendo los endpoints administrativos y los datos editoriales.

### 3. Arquitectura Escalable

Sigue una estructura modular basada en componentes diseñada para alta disponibilidad y separación de responsabilidades. El tipado estricto y los patrones estandarizados de React aseguran ciclos de mantenimiento predecibles.

---

## 🏗️ Visión General de la Arquitectura

```text
venezuela-news-app/
├── src/
│   ├── app/                 # Next.js App Router & Server Components
│   │   ├── (cms)/           # Rutas Administrativas Protegidas
│   │   ├── (marketing)/     # Rutas de Acceso Público (Landing & Feed)
│   │   └── actions/         # Next.js Server Actions (Lógica Backend)
│   ├── components/          # Componentes Modulares de React (UI & Features)
│   ├── lib/                 # Utilidades Core, Clientes API & Hooks
│   └── types/               # Definiciones e Interfaces de TypeScript
```

**Stack Tecnológico Enterprise:**

- **Framework:** Next.js (App Router, Server Components)
- **Estilos & UI:** Tailwind CSS, Framer Motion, Radix Primitives
- **Capa de Datos:** Supabase (PostgreSQL, Auth, Storage)
- **Motor:** TypeScript (Modo Estricto)

---

## ⚙️ Instalación y Desarrollo

Asegúrate de tener instalado `Node.js 18+`.

1. **Clonar el repositorio:**

   ```bash
   git clone https://github.com/LuisSambrano/venezuela-news-app.git
   ```

2. **Instalar dependencias:**

   ```bash
   cd venezuela-news-app
   npm install
   ```

3. **Configurar Variables de Entorno:**
   Crea un archivo `.env.local` en la raíz del proyecto y añade tus claves de Supabase:

   ```env
   NEXT_PUBLIC_SUPABASE_URL=tu-url-de-supabase
   NEXT_PUBLIC_SUPABASE_ANON_KEY=tu-anon-key-de-supabase
   ```

4. **Ejecutar el servidor local de desarrollo:**
   ```bash
   npm run dev
   ```

---

## 🎨 Estándares de Código

Este repositorio aplica estándares de ingeniería estrictos:

1. `npm run lint` debe resultar en cero errores o advertencias antes de cada commit.
2. `tsc --noEmit` debe pasar sin errores de tipado.
3. No se permiten tipos `any`; usa tipado estricto o `unknown` con Type Guards.
4. Se requieren Conventional Commits para el control de versiones.

---

## 📄 Licencia y Contribución

Este proyecto es propietario. Por favor, consulta `.agent/rules/PROTOCOL_ZERO.md` para las pautas arquitectónicas internas.
