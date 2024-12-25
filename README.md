# React TypeScript Visual Studio Code Template

A minimal React SWC Vite starter template with Prettier plugin integration and basic settings for Visual Studio Code.

## Feature

- ⚡️ Fast - Build tools based on vite.
- ⏱️ Small - Based on the smallest runnable build.
- 🎈 Prettier - Integrated Prettier to help you format the code.
- 😎 Reliable - Integrated eslint.

## Getting Started

```bash
npx degit iwebexpert/vite-react-swc-ts-vscode app
cd app
git init
```

### Prerequisites

- `npm` and `pnpm` should be installed.
- `git` should be installed (recommended v2.4.11 or higher)

## Branch pnpm-only

The pnpm-only branch enforces the use of pnpm through the **"preinstall": "npx only-allow pnpm"** script.

### Creating an Application from the pnpm-only branch

Follow these steps to create a new application from the pnpm-only branch:

```bash
# Create the application using degit with the specified branch
npx degit iwebexpert/vite-react-swc-ts-vscode#pnpm-only app

cd app
pnpm install
git init
```

## Enabling pnpm with Corepack

Corepack is included by default in recent versions of Node.js. To enable pnpm globally using Corepack:

```bash
corepack enable

# Ensure pnpm is activated
corepack prepare pnpm@latest --activate

# Verify pnpm is working
pnpm --version
```

### Available scripts

#### `pnpm dev`

Runs the app in development mode.
Open https://localhost:5173 to view it in the browser.

The page will automatically reload if you make changes to the code.
You will see the build errors and lint warnings in the console.

#### `pnpm build`

Builds the app for production to the `dist` folder.
It correctly bundles React in production mode and optimizes the build for the best performance.
