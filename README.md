# shadcn/ui monorepo template

This template is for creating a monorepo with shadcn/ui. Shadcn provides a pnpm sample which breaks because users do not have pnpm installed - this repository has the necessary changes to run the monorepo with npm instead.

The repo consist of:
- Tailwind CSS
- NextJS web app (more apps can be installed in the apps folder)
- Shadcn components
- Typescript
- npm package manager

## Running The Project
In the root folder run:
```bash
npm install
```
Then run:
```bash
npm run dev
```

## Adding components

To add components to your app, make sure to cd into the relevant app and then run the install command as per shadcn documentation:

```bash
cd apps/web
npx shadcn@canary add [COMPONENT]
```

This will place the ui components in the `packages/ui/src/components` directory.

## Tailwind

Your `tailwind.config.ts` and `globals.css` are already set up to use the components from the `ui` package.

## Using components

To use the components in your app, import them from the `ui` package.

```tsx
import { Button } from "@workspace/ui/components/button"
```
