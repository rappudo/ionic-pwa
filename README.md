# ionic-pwa (Anime Catalog)

A social anime catalog built as a Progressive Web App.

> Coursework · Mobile Programming · 2026-1 · finished

## Goal
Build a PWA that works offline and still has a social layer: the anime catalog is
static JSON cached by the service worker, while ratings, lists, friendships and
recommendations live in Supabase, protected by Row Level Security.

## Stack
- Angular 20, Ionic 8, Capacitor 8
- Angular service worker (PWA), RxJS + signals
- Supabase (Postgres, Auth, Storage, RLS)
- Karma + Jasmine, ESLint

## How to run
```bash
npm install
npm start                                          # http://localhost:4200
npm run build && npx http-server www -p 8080 -c-1  # real PWA, service worker on
```
Supabase settings: `src/environments/environment.ts`.

## What I took from it
- How a PWA is structured (service worker, manifest, offline cache).
- Angular, and building the frontend out of reusable components.
- Web development in general, and frontend for mobile devices.
