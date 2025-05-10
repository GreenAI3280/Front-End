/*
README for Front-end – React 18 + Vite + TailwindCSS

Overview
--------
This is a minimal, practical React 18 single-page application scaffolded with Vite and styled using TailwindCSS. It demonstrates a responsive dashboard layout with a header and card components.

Requirements
------------
- Node.js >= 14
- npm or yarn

Installation
------------
1. Initialize a new Vite + React + TS project:
   ```bash
   npm create vite@latest my-app -- --template react-ts
   cd my-app
   ```
2. Install dependencies:
   ```bash
   npm install
   npm install -D tailwindcss postcss autoprefixer
   npx tailwindcss init -p
   ```
3. Replace project files with the ones below.  
4. Start development server:
   ```bash
   npm run dev
   ```
5. Build for production:
   ```bash
   npm run build
   ```

Project Structure
-----------------
- `package.json`      – add Tailwind and autoprefixer
- `vite.config.ts`    – Vite config with React plugin
- `tailwind.config.js` – Tailwind content paths
- `postcss.config.js` – PostCSS plugins
- `index.html`        – root HTML
- `src/index.css`     – Tailwind directives
- `src/main.tsx`      – React entry point
- `src/App.tsx`       – Main component

---

// vite.config.ts
import { defineConfig } from 'vite';
import react from '@vitejs/plugin-react';

export default defineConfig({
  plugins: [react()],
});
