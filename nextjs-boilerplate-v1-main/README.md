# Zing7 Next.js 14.2.3 boilerplate

## 1. Bootstrapping

This project was created with `bun create next-app`. In a nutshell, you can use bun just like npm, but it's faster. [Check bun here](https://bun.sh/)

Install wizard steps.

```sh
❯ bun create next-app
✔ What is your project named? … ./
✔ Would you like to use TypeScript? … No / Yes -> Yes
✔ Would you like to use ESLint? … No / Yes -> Yes
✔ Would you like to use Tailwind CSS? … No / Yes -> yes
✔ Would you like to use `src/` directory? … No / Yes -> Yes
✔ Would you like to use App Router? (recommended) … No / Yes -> Yes
✔ Would you like to customize the default import alias (@/*)? … No / Yes -> No
```

## 2. Running the project project

- Run `npm install` | `yarn install` | `bun install` | `pnpm install`
- Then run `bun dev` | `yarn dev` | `npm run dev` | `pnpm run dev`
- Visit [http://localhost:3000](http://localhost:3000) or [http://0.0.0.0:3000](http://0.0.0.0:3000)

## 3. Project structure

```
├── node_modules - package folder
├── public - public assets like images, routes remapped to the root:
│   ├── next.svg - Link for asset is /next.svg (<img src="/next.svg" />)
├── src
│   ├── app
│   │   ├── https://nextjs.org/docs/getting-started/project-structure
│   │   ├── page.tsx - where your page is
│   │   ├── layout.tsx - where your layout is
│   │   ├── loading.tsx - global suspense boundry loading
│   │   ├── global-error.tsx - custom 500 page. If there is an error, display custom content
│   │   ├── not-found.tsx - custom 404 page
│   │   ├── route.tsx - if the route is an API route
│   ├── components
│   │   ├── ui - reusable components
│   │   ├── layout - layout components - header, footer, main, etc.
│   ├── config
│   │   ├── constants.ts - global constants file
│   ├── hooks - folder where all the hooks live
│   │   ├── use-mounted.ts - a hook for checking mouted state
│   ├── lib - folder where all your services should live. (access to database, server actions, etc.)
│   │   ├── utils.ts - utility functions
│   ├── providers - folder where all your context providers live
│   │   ├── theme-provider.tsx - Provider for dark mode
├── .eslint.json - config for eslint rules
├── .gitignore - where you ignore files
├── .prettierrc - config for prettier extenstion that formats code
├── next-env.d.ts - environment ts vars for nextjs. Do not edit this file. It will be overwritten
├── next.config.mjs - configuration for next.js
├── package.json - project config
├── package-lock.json - the lock file for installed packages
├── postcss.config.mjs - instructions to postcss on how to modify and purge unused styles
├── tailwind.config.ts - config for the tailwindcss dep
└── tsconfig.json - configuration for TypeScript
```

## 4. Hints

- Tailwind has custom styles in config, check tailwindconfig
- tsconfig has modified paths, check tsconfig
- a theme switcher is installed, check providers.
- a tailwind merger func is installed, check lib/utils