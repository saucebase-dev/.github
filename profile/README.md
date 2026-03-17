<div align="center">
  <a href="https://saucebase-dev.github.io/docs/">
    <img src="https://github.com/saucebase-dev/saucebase/raw/main/public/images/logo.svg" alt="Saucebase" width="200" />
  </a>

  <h1>Saucebase</h1>

  <p>An enterprise-grade, modular Laravel SaaS starter kit. Own your code, ship faster.</p>

  <p>
    <a href="https://github.com/saucebase-dev/saucebase/actions/workflows/test.yml"><img src="https://github.com/saucebase-dev/saucebase/actions/workflows/test.yml/badge.svg" alt="Tests" /></a>
    <a href="https://github.com/saucebase-dev/saucebase/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License" /></a>
    <a href="https://php.net"><img src="https://img.shields.io/badge/PHP-8.4%2B-777BB4?logo=php&logoColor=white" alt="PHP Version" /></a>
    <a href="https://laravel.com"><img src="https://img.shields.io/badge/Laravel-12.0-FF2D20?logo=laravel&logoColor=white" alt="Laravel" /></a>
    <a href="https://vuejs.org"><img src="https://img.shields.io/badge/Vue.js-3.4-4FC08D?logo=vue.js&logoColor=white" alt="Vue.js" /></a>
    <a href="https://typescriptlang.org"><img src="https://img.shields.io/badge/TypeScript-5.8-3178C6?logo=typescript&logoColor=white" alt="TypeScript" /></a>
    <a href="https://vitejs.dev"><img src="https://img.shields.io/badge/Vite-6.4-646CFF?logo=vite&logoColor=white" alt="Vite" /></a>
    <a href="https://tailwindcss.com"><img src="https://img.shields.io/badge/Tailwind%20CSS-4.1-06B6D4?logo=tailwind-css&logoColor=white" alt="Tailwind CSS" /></a>
    <a href="https://inertiajs.com"><img src="https://img.shields.io/badge/Inertia.js-2.0-9553E9?logo=inertia&logoColor=white" alt="Inertia.js" /></a>
    <a href="https://filamentphp.com"><img src="https://img.shields.io/badge/Filament-5.0-10B981?logo=filament&logoColor=white" alt="Filament" /></a>
    <a href="https://playwright.dev"><img src="https://img.shields.io/badge/Playwright-1.40-000000?logo=playwright&logoColor=white" alt="Playwright" /></a>
    <a href="https://phpstan.org"><img src="https://img.shields.io/badge/PHPStan-level%205-brightgreen.svg?style=flat" alt="PHPStan" /></a>
  </p>

  <img src="https://github.com/saucebase-dev/saucebase/raw/main/public/images/screenshots/preview.gif" alt="Saucebase preview" width="700" />

  <p>
    Built on the <strong>VILT stack</strong> (Vue 3, Inertia.js, Laravel 12, Tailwind CSS 4) with TypeScript, SSR support,
    and a copy-and-own module system inspired by shadcn/ui. Install only what you need, customize everything,
    no vendor lock-in.
  </p>

  <p>
    <a href="https://demo.saucebase.dev/"><strong>Online Demo</strong></a> ·
    <a href="https://saucebase-dev.github.io/docs/"><strong>Documentation</strong></a> ·
    <a href="https://github.com/saucebase-dev/saucebase/issues"><strong>Report a Bug</strong></a> ·
    <a href="https://github.com/saucebase-dev/saucebase/discussions"><strong>Discussions</strong></a>
  </p>
</div>

---

## What is Saucebase?

Saucebase is a production-ready Laravel SaaS starter kit that gives you **complete ownership of your code**. Unlike traditional starter kits that trap you in vendor packages, Saucebase uses a **copy-and-own philosophy** — modules install directly into your repository, not as external dependencies you can't modify.

When you install a Saucebase module, the source code lands in your `modules/` directory. You can open any file and change it. No patches, no overrides, no fighting against package assumptions.

> **You are the vendor.** From day one, you control the roadmap, the updates, and the architecture.

---

## Key Features

- 🧩 **Modular Architecture** — self-contained feature modules that copy into your codebase; each includes routes, controllers, models, migrations, Vue pages, and tests
- ⚡ **One-command setup** — Docker, Herd, Sail, and native PHP all supported; get running in minutes
- 🔁 **No API layer needed** — Inertia.js connects Laravel controllers directly to Vue components with full TypeScript type safety
- 🔍 **SSR on demand** — opt-in server-side rendering per page for SEO-critical routes
- 🏗️ **Production-ready tooling** — PHPStan level 5, Laravel Pint, ESLint, Playwright E2E, commitlint
- 🎨 **Beautiful UI** — [shadcn-vue](https://www.shadcn-vue.com/) components with Tailwind CSS 4 and dark mode out of the box
- 🛡️ **Admin panel** — Filament 5 included with user management and module-specific resources

---

## Technology Stack

| Layer | Technologies |
|---|---|
| **Backend** | Laravel 12 · PHP 8.4+ · Filament 5 · Spatie Permission |
| **Frontend** | Vue 3 · TypeScript 5.8 · Inertia.js 2.0 · shadcn-vue |
| **Styling** | Tailwind CSS 4 · Reka UI · Lucide icons |
| **Database** | MySQL · Redis |
| **Testing** | Playwright (E2E) · PHPUnit |
| **Dev Tools** | Vite 6 · PHPStan · Laravel Pint · ESLint · Prettier · Husky |
| **Infrastructure** | Docker · Nginx · Mailpit |

---

## Modules

Modules are self-contained features that copy directly into your repository — you own every line. Each module ships with its own routes, controllers, models, migrations, Vue pages, and tests.

### 🔐 [Auth](https://github.com/saucebase-dev/auth)
Complete authentication: email/password, password reset, email verification, social login (Google & GitHub via OAuth), provider connect/disconnect, and admin user impersonation. Includes a Filament admin panel at `/admin`.

### ⚙️ [Settings](https://github.com/saucebase-dev/settings)
User profile management: edit name/email, upload an avatar, change password, and manage connected OAuth providers. Requires the Auth module.

### 💳 [Billing](https://github.com/saucebase-dev/billing)
Stripe-powered subscriptions: checkout sessions, subscription management, billing portal, invoice list, and webhook processing. Gateway driver pattern supports Paddle and LemonSqueezy too. Requires the Auth module.

### 📢 [Announcements](https://github.com/saucebase-dev/announcements)
Site-wide announcement banners: rich text, scheduling, audience targeting (guests/authenticated/all), and cookie-based dismissal. Managed via Filament admin at `/admin`.

### 🧭 [Roadmap](https://github.com/saucebase-dev/roadmap)
The Roadmap module gives authenticated users a page to suggest features or bugs, vote on what matters most, and see where things stand. New suggestions go through a moderation step before they become visible to others.
---

## Documentation

Full installation guides, configuration reference, architecture deep-dives, and development workflows are maintained in the **[Saucebase Documentation](https://saucebase-dev.github.io/docs/)** — the single source of truth.

---

## Repositories

| Repository | Description |
|---|---|
| [saucebase-dev/saucebase](https://github.com/saucebase-dev/saucebase) | Main application |
| [saucebase-dev/auth](https://github.com/saucebase-dev/auth) | Auth module |
| [saucebase-dev/settings](https://github.com/saucebase-dev/settings) | Settings module |
| [saucebase-dev/billing](https://github.com/saucebase-dev/billing) | Billing module |
| [saucebase-dev/announcements](https://github.com/saucebase-dev/announcements) | Announcements module |
| [saucebase-dev/docs](https://github.com/saucebase-dev/docs) | Documentation site |
| [saucebase-dev/laravel-playwright](https://github.com/saucebase-dev/laravel-playwright) | Laravel + Playwright integration |

---

## License

Saucebase is open-source software licensed under the [MIT license](https://opensource.org/licenses/MIT).
