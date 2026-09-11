---
description: 'Tailwind CSS v4 styling patterns and dark theme guidelines'
applyTo: '**/*.{astro,css}'
---

# Tailwind CSS Instructions

## Tailwind CSS v4 Configuration

This project uses Tailwind CSS v4.1.14 via the `@tailwindcss/vite` plugin.

### Global CSS Setup

- Import Tailwind in `global.css`: `@import "tailwindcss";`
- No separate `tailwind.config.js` file is used
- Configuration is handled through the Vite plugin

## Dark Theme Styling

ALL UI components MUST use dark theme colors:

### Color Palette

- Background colors: `bg-slate-800`, `bg-slate-900`, `bg-slate-950`
- Text colors: `text-slate-100`, `text-slate-200`, `text-slate-300`
- Border colors: `border-slate-700`, `border-slate-600`
- Accent colors for hover/focus states

### Common Patterns

- Cards and containers: `bg-slate-800 rounded-xl p-6 shadow-lg`
- Hover effects: `hover:bg-slate-700 transition-colors duration-200`
- Borders: `border border-slate-700`
- Gradients for visual interest: `bg-gradient-to-br from-slate-800 to-slate-900`
- Backdrop effects: `backdrop-blur-sm bg-slate-900/50`

### Responsive Design

- Use responsive prefixes: `sm:`, `md:`, `lg:`, `xl:`
- Mobile-first approach
- Ensure readability on all screen sizes

## Utility Classes

- Prefer utility classes over custom CSS when possible
- Use semantic grouping: layout, spacing, colors, typography
- Keep utility combinations readable and maintainable

## TypeScript and comment conventions

- Use explicit TypeScript parameter and return types, especially for exported helpers and public component props.
- Prefer `interface`/`type` declarations for object shapes and avoid `any` in application code; the lint rules enforce `@typescript-eslint/no-explicit-any` where possible.
- Keep comments focused on intent, assumptions, and edge cases rather than re-stating the code. If a comment no longer matches the implementation, update or remove it with the change that caused the mismatch.

## Modern UI Patterns

- Rounded corners: `rounded-lg`, `rounded-xl`, `rounded-2xl`
- Smooth transitions: `transition-all duration-200 ease-in-out`
- Shadows for depth: `shadow-md`, `shadow-lg`, `shadow-xl`
- Focus states for accessibility: `focus:ring-2 focus:ring-blue-500`
