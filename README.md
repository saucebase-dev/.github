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

## Why Saucebase?

Most Laravel starter kits force you to choose between convenience and control. You either accept their rigid architecture or maintain a messy fork. Saucebase eliminates this trade-off.

| Traditional Starter Kits | Saucebase |
|---|---|
| Code locked in `vendor/` | Code in your `modules/` directory |
| Can't modify without patching | Edit files directly — you own them |
| Upstream updates can break your app | You control when and how things change |
| Fight the package's assumptions | Customize freely to match your architecture |
| Vendor controls your roadmap | You control your roadmap |

---

## Key Features

### 🧩 Modular Architecture
Self-contained feature modules that copy into your codebase. Each module includes its own routes, controllers, models, migrations, Vue pages, and tests. Enable only what you need.

### ⚡ Modern Development Experience
- **One-command setup** — `bash bin/setup-env` starts Docker containers, configures your database, generates SSL certificates, and builds assets automatically
- **Instant hot reload** — Vite HMR means you see changes immediately without page refresh
- **Type-safe routes** — Ziggy generates TypeScript helpers from your Laravel routes, giving you autocomplete and type checking across the stack
- **SSR on demand** — opt-in server-side rendering per page for SEO-critical pages

### 🏗️ Production Ready
- **PHPStan level 5** static analysis on all PHP code
- **Laravel Pint** + ESLint for consistent code style
- **Playwright** E2E testing pre-configured with Laravel integration
- **Commitlint** for conventional commit messages
- **Filament 5** admin panel included

### 🎨 Beautiful UI Components
Built with [shadcn-vue](https://www.shadcn-vue.com/) — accessible, customizable components using Tailwind CSS 4 and Reka UI. Dark mode supported out of the box.

---

## Technology Stack

| Layer | Technologies |
|---|---|
| **Backend** | Laravel 12 · PHP 8.4+ · Filament 5 (admin panel) · Spatie Permission |
| **Frontend** | Vue 3 Composition API · TypeScript 5.8 · Inertia.js 2.0 |
| **Styling** | Tailwind CSS 4 · shadcn-vue · Lucide icons |
| **Database** | MySQL · Redis (cache, sessions, queues) |
| **Testing** | Playwright (E2E) · PHPUnit (backend) |
| **Dev Tools** | Vite 6 · PHPStan · Laravel Pint · ESLint · Prettier · Husky |
| **Infrastructure** | Docker · Nginx · Mailpit (local email) |

---

## Quick Start

### Docker (recommended)

Only Docker Desktop and Node.js 22+ are required.

```bash
git clone https://github.com/saucebase-dev/saucebase.git my-app
cd my-app
bash bin/setup-env
```

Visit **https://localhost** when the setup completes. The bootstrap script handles everything: starts Docker containers (MySQL, Redis, Mailpit), installs dependencies, runs migrations, enables modules, and builds frontend assets.

### Laravel Herd

```bash
git clone https://github.com/saucebase-dev/saucebase.git my-app
cd my-app
composer install
cp .env.example .env
# Set APP_URL to your Herd site URL in .env
# Configure DB_* credentials in .env
php artisan saucebase:install
npm install && npm run dev
```

### Laravel Sail

```bash
git clone https://github.com/saucebase-dev/saucebase.git my-app
cd my-app
cp .env.example .env
# Configure .env for Sail (DB_HOST=mysql, REDIS_HOST=redis, etc.)
sail up -d
sail composer install
sail artisan saucebase:install
npm install && npm run dev
```

### Native PHP

```bash
git clone https://github.com/saucebase-dev/saucebase.git my-app
cd my-app
composer install
cp .env.example .env
# Configure APP_URL, DB_*, REDIS_* in .env
php artisan saucebase:install
npm install && npm run dev
```

### Default Credentials

After running the installer with the Auth module:

- **Email:** `chef@saucebase.dev`
- **Password:** `secretsauce`

> ⚠️ Change these before going to production.

---

## Installer Options

```bash
php artisan saucebase:install [options]
```

| Flag | Description |
|---|---|
| _(none)_ | Interactive: `migrate --seed`, prompts for module selection |
| `--fresh` | Runs `migrate:fresh --seed` — **drops all tables first** |
| `--all-modules` | Enable and migrate all discovered modules automatically |
| `--modules=Auth,Settings` | Enable specific modules only |
| `--force` | Skip confirmations |
| `--no-interaction` | Non-interactive mode (selects all modules automatically) |

---

## Available Modules

Modules are self-contained features that install directly into your repository. Installing a module is as simple as:

```bash
composer require saucebase/<module-name>
php artisan module:enable <ModuleName>
php artisan module:migrate <ModuleName> --seed
npm run build
```

### 🔐 [Auth](https://github.com/saucebase-dev/auth)

Complete authentication system built on top of Laravel's built-in auth.

- Email/password login and registration with rate limiting
- Password reset via email
- Email verification with resend support
- **Social login (OAuth)** — Google and GitHub via Laravel Socialite
- Provider connect/disconnect with safety guards
- **Admin impersonation** — admins can impersonate any user from the Filament panel
- Filament admin panel (`/admin`) with full user management

### ⚙️ [Settings](https://github.com/saucebase-dev/settings)

User profile management (requires Auth module).

- Edit profile — name, email
- Avatar upload (JPEG, PNG, GIF, WebP; max 2 MB) via Spatie Media Library
- Avatar fallback — social provider photo, then default avatar
- Password change with confirmation email
- Social provider connect/disconnect from profile page

### 💳 [Billing](https://github.com/saucebase-dev/billing)

Subscription management and payment processing (requires Auth module).

- Stripe checkout flow with configurable session expiry
- Cancel at period end and resume before expiry
- Stripe-hosted billing portal (update card, download invoices)
- Invoice list with status indicators
- Webhook processing with idempotency via `webhook_events` table
- Gateway driver pattern — Stripe by default, Paddle and LemonSqueezy configurable
- Automatic `subscriber` role management via Spatie Permission
- Pricing section component for your landing page

### 📢 [Announcements](https://github.com/saucebase-dev/announcements)

Site-wide announcement banners (requires Auth module).

- Fixed banner at the top of every page, above the navigation
- Rich text content — bold, italic, links, lists
- Scheduling with `starts_at` / `ends_at`
- Audience targeting — public pages, authenticated pages, or both
- Cookie-based dismissal (SSR-safe, no database writes)
- Filament admin CRUD at `/admin`

---

## Architecture

Saucebase follows the **VILT stack** pattern: Vue 3 as the frontend, Inertia.js as the glue, Laravel as the backend, and Tailwind CSS for styling.

```
Browser ──HTTPS──► Laravel (routes + controllers)
                        │
                        ▼
                   Inertia Response (JSON)
                        │
                        ▼
              Vue 3 (renders page component)
                   ▲         │
                   │         ▼
              SPA navigation  Props (typed with TypeScript)
```

### No API Layer Needed

Inertia.js lets your controllers pass data directly to Vue components as typed props — no REST API, no GraphQL, no manual serialization.

```php
// Laravel controller
return Inertia::render('Dashboard', [
    'stats' => $stats,
    'user'  => $user,
]);
```

```typescript
// Vue component — fully typed
const props = defineProps<{ stats: Stats; user: User }>();
```

### Module Structure

Each module lives in `modules/<Name>/` with a predictable layout:

```
modules/Auth/
├── config/           # Module configuration
├── database/
│   ├── factories/    # Model factories
│   ├── migrations/   # Database migrations
│   └── seeders/      # Database seeders
├── patches/          # Git patches for core app integration
├── resources/
│   └── js/           # Vue pages and components
├── routes/           # Web routes
├── src/              # PHP source (Controllers, Models, etc.)
└── tests/            # Feature and E2E tests
```

### SSR (Opt-In)

Server-side rendering is available but disabled by default. Enable it per-route for SEO-critical pages:

```php
return Inertia::render('Products/Index')->withSSR();  // SSR on
return Inertia::render('Dashboard');                  // SSR off (default)
```

---

## Development Commands

### Frontend

```bash
npm run dev          # Start Vite dev server with HMR
npm run build        # Build for production (includes SSR build)
npm run format       # Format code with Prettier
npm run lint         # Lint and auto-fix with ESLint
```

### Backend (Docker)

```bash
docker compose exec app php artisan <command>
docker compose exec app composer <command>
```

### Testing

```bash
# Backend tests
php artisan test

# E2E tests (Playwright)
npx playwright test
npx playwright test --ui            # Interactive UI mode
npx playwright test --headed        # Headed browser mode

# Module-specific tests
php artisan test --testsuite=Modules --filter=Auth
npx playwright test --project="@Auth*"
```

### Module Management

```bash
php artisan module:list                          # List all modules and their status
php artisan module:enable <ModuleName>           # Enable a module
php artisan module:disable <ModuleName>          # Disable a module
php artisan module:migrate <ModuleName> --seed   # Run module migrations
```

---

## Directory Structure

```
saucebase/
├── app/                    # Core Laravel application
│   ├── Http/               # Controllers, Middleware
│   ├── Models/             # Eloquent models
│   └── Providers/          # Service providers
├── bin/
│   └── setup-env           # Docker bootstrap script
├── docker/                 # Docker configuration
├── modules/                # Installed Saucebase modules
│   ├── Auth/               # Authentication module
│   ├── Settings/           # User settings module
│   ├── Billing/            # Billing/subscription module
│   └── Announcements/      # Announcement banners module
├── resources/
│   └── js/
│       ├── components/     # Shared Vue components (shadcn-vue)
│       ├── layouts/        # Page layouts
│       ├── pages/          # Core application pages
│       └── types/          # TypeScript type definitions
├── routes/                 # Application routes
└── tests/                  # Core application tests
```

---

## Configuration

Key environment variables unique to Saucebase:

| Variable | Description |
|---|---|
| `APP_URL` | Full URL including protocol — **must be set before install** |
| `APP_HOST` | Hostname portion (e.g. `localhost`, `my-app.test`) |
| `APP_SLUG` | Project slug for storage/cache keys — don't change after deploy |
| `VITE_LOCAL_STORAGE_KEY` | Frontend localStorage prefix (defaults to `APP_SLUG`) |
| `BILLING_GATEWAY` | Payment gateway: `stripe` (default), `paddle`, `lemonsqueezy` |
| `STRIPE_SECRET_KEY` | Stripe secret key (Billing module) |
| `STRIPE_PUBLISHABLE_KEY` | Stripe publishable key (Billing module) |
| `STRIPE_WEBHOOK_SECRET` | Stripe webhook signing secret (Billing module) |
| `GOOGLE_CLIENT_ID` | Google OAuth client ID (Auth module) |
| `GITHUB_CLIENT_ID` | GitHub OAuth client ID (Auth module) |

---

## Docker Services

When using the Docker setup, the following services are available:

| Service | Purpose | Default Port |
|---|---|---|
| **nginx** | Web server with SSL | 80, 443 |
| **app** | PHP-FPM + CLI | — |
| **mysql** | Database | 3306 |
| **redis** | Cache / Queue / Sessions | 6379 |
| **mailpit** | Local email testing UI | 8025 |

---

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch: `git checkout -b feat/your-feature`
3. Make your changes following the coding standards
4. Run tests: `php artisan test` and `npx playwright test`
5. Commit using conventional commits: `git commit -m "feat: add your feature"`
6. Open a pull request

### Coding Standards

- PHP: [Laravel Pint](https://laravel.com/docs/pint) + PHPStan level 5
- TypeScript/Vue: ESLint + Prettier
- Commits: [Conventional Commits](https://www.conventionalcommits.org/) enforced by commitlint

---

## Related Repositories

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