This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!


## Project Structure
/
├── .env                  # Environment variables
├── .env.local            # Local development env
├── next.config.js
├── package.json
├── sentry.client.config.ts # Sentry client config
├── sentry.server.config.ts # Sentry server config
├── tsconfig.json
│
├── /app/                 # Next.js App Router (src/app if using src structure)
│   ├── /(auth)/          # Public auth routes (sign-in, sign-up, etc.)
│   ├── /dashboard/       # Protected application area
│   └── /api/             # API routes
│
├── /components/          # Shared and reusable React components
│   ├── /ui/              # General-purpose UI elements (e.g., from shadcn/ui)
│   ├── /forms/           # Reusable form components
│   └── /layout/          # Layout components (Sidebar, Topbar, etc.)
│
├── /features/            # Business logic and hooks, organized by feature
│   ├── /auth/            # Authentication logic and Supabase helpers
│   ├── /billing/         # Stripe and billing management logic
│   ├── /settings/        # User settings logic
│   └── ...
│
├── /hooks/               # General-purpose reusable hooks
│
├── /lib/                 # Library initializations and core helpers
│   ├── /supabase/        # Supabase client and admin client setup
│   ├── /stripe/          # Stripe client and webhook handlers
│   └── /api/             # API helpers (e.g., TRPC client, fetcher)
│
├── /public/              # Static assets (images, fonts, etc.)
│
├── /store/               # Global state management (Zustand)
│
├── /styles/              # Global CSS styles
│
├── /types/               # Global TypeScript type definitions
│
└── /utils/               # General utility functions (formatting, validation, etc.)



## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.
