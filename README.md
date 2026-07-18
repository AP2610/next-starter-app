# Next.js Starter Template

A Next.js starter template designed to help me get up and running quickly with all the essential tools and configurations pre-setup.

Why?

I spend a good amount of time setting up my project before I can actually start diving into the code and building something. The goal of this starter template is to have that all done for me already.

I also created a small package to be able to quickly get a new project running using `npx`.

## Getting Started

```bash
# Run
npx create-next-starter-app-template

# Start development server
pnpm dev
```

### Core Framework

- **Next.js 16** with App Router
- **React 19**
- **TypeScript**
- **Tailwind CSS v4**

### Styling & UI

- **Google Fonts** Raleway & Montserrat by default, change in layout
- **Motion** for animations

### Existing Components

- **Section Layout Component** with a scroll animation

### Existing Hooks

- **Media query hook** for responsive logic

### Development Tools

- **ESLint** with TypeScript and Prettier integration, set according to my preferences
- **Prettier** with Tailwind CSS plugin
- **Husky** for git hooks, primarily for linting and running tests pre-commit
- **lint-staged** for pre-commit formatting

### Testing Setup

- Vitest with React Testing Library
- Coverage reporting

### Utilities

- Date formatting utilities
- Debounce utility
- Class merging utility - (`cn`) for conditional styling

### Structure

```
src/
├── app/                 # Next.js App Router
├── components/          # Reusable components
│   ├── features/        # Feature-specific components
│   ├── layout/          # Layout components
│   └── ui/              # UI components
├── hooks/               # Custom React hooks
├── lib/                 # Utilities and helpers
│   ├── stores/          # State management
│   ├── types/           # TypeScript types
│   └── utils/           # Utility functions
├── server-actions/      # Server actions
├── server-functions/    # Server functions
└── styles/              # Global styles
```

## Customization

### Colors

Update the color palette in `src/styles/globals.css`:

```css
@theme {
  /* Add your custom colors here */
}

@theme inline {
  /* Add custom variables referencing variables defined in @theme */
}
```

### Fonts

Change fonts in `src/app/layout.tsx`:

```tsx
import { YourFont } from 'next/font/google';
```

## Dependencies

I'm placing these here in case I need to quickly use them in a project not using this template.

### UI & Styling

- `motion@12.42.2`
- `react-icons@5.7.0`
- `clsx@2.1.1`
- `tailwind-merge@3.6.0`

### Development

- `prettier@3.9.5`
- `prettier-plugin-tailwindcss`
- `husky@9.1.7`
- `vitest@4.1.10`
- `@vitest/coverage-v8`
- `@vitejs/plugin-react`
- `jsdom`
- `@testing-library/dom`
- `@testing-library/jest-dom`
- `@testing-library/react@16.3.0`
- `@typescript-eslint/eslint-plugin`
- `@typescript-eslint/parser`
- `eslint-config-prettier`
- `eslint-plugin-prettier`
