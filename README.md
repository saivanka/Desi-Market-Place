# Desi Market Place

A marketplace web app for browsing listings, managing your own listings and saving favorites, backed by Supabase. The deployed site is https://desimarketplace.vercel.app.

## What it does

- Home page listing feed (`/`)
- My Listings page (`/my-listings`) for managing listings you posted
- Favorites page (`/favorites`) for saved listings
- Profile page is currently a coming-soon placeholder (`/profile`)
- Toast notifications via shadcn/ui and Sonner

## Tech stack

- React 18 + TypeScript + Vite, React Router, TanStack Query, React Hook Form + Zod
- shadcn/ui on Radix UI primitives, Tailwind CSS
- Supabase for backend data and auth (`src/integrations/supabase`, `@supabase/supabase-js`, `@supabase/auth-ui-react`)

## How to run

```bash
npm install
npm run dev      # vite
npm run build    # vite build
npm run preview  # vite preview
```

## Project structure

```
src/App.tsx                  # Routes: /, /my-listings, /favorites, /profile, catch-all
src/pages/                   # Index, MyListings, Favorites, ComingSoon, NotFound
src/components/              # UI components (incl. ui/ shadcn components)
src/hooks/                   # Custom hooks
src/integrations/supabase/   # Supabase client integration
src/lib/                     # Shared utilities
index.html                   # Entry HTML
```
