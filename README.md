# shadcn/ui monorepo template

This template is for creating a monorepo with shadcn/ui. shadcn provides a pnpm sample - this repository has the necessary changes to run the monorepo with npm instead of pnpm.

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
