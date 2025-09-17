# Wall & Fifth — AI & Software Products (Next.js App Router)

A clean, fast website for **Wall & Fifth** as a **parent company** that builds products (apps + AI).  
The site centers on **your products** (not services), with crisp sections, good SEO, and an easy deploy path.

---

## Tech Stack
- **Next.js (App Router)** + **TypeScript**
- **Tailwind v4** (via `@import "tailwindcss"` in `app/globals.css`)
- Icons: **lucide-react** (optional)
- Zero heavy animation deps (tiny in-view helper)
- First-party SEO routes (`app/sitemap.ts`, `app/robots.ts`)

> Fonts wired via `app/layout.tsx` (Inter Tight + Instrument Serif).  
> Global tokens/utilities in `app/globals.css`.

---

## Quickstart

```bash
# install deps
pnpm i         # or npm i / yarn

# run dev server
pnpm dev       # http://localhost:3000

# build & start
pnpm build && pnpm start
Environment (recommended):

ini
Copy code
# .env.local
NEXT_PUBLIC_SITE_URL=https://your-domain.com
Project Structure
python
Copy code
.
├─ app/
│  ├─ layout.tsx
│  ├─ globals.css
│  ├─ page.tsx
│  ├─ not-found.tsx
│  ├─ about/
│  │  └─ page.tsx
│  ├─ press/
│  │  └─ page.tsx
│  ├─ products/
│  │  ├─ page.tsx
│  │  └─ [slug]/
│  │     └─ page.tsx
│  ├─ product/
│  │  └─ page.tsx        # redirect → /products
│  ├─ projects/
│  │  └─ [slug]/
│  │     └─ page.tsx     # optional case studies (reads /data/projects.ts)
│  ├─ sitemap.ts
│  └─ robots.ts
│
├─ components/
│  ├─ Header.tsx
│  ├─ Footer.tsx
│  ├─ MotionRoot.tsx
│  ├─ Hero.tsx
│  ├─ Products.tsx
│  ├─ Approach.tsx
│  ├─ Capabilities.tsx
│  ├─ Clients.tsx
│  ├─ Changelog.tsx
│  ├─ FAQ.tsx
│  ├─ CTA.tsx
│  ├─ Contact.tsx
│  └─ Projects.tsx       # not on the homepage anymore
│
├─ data/
│  ├─ products.ts
│  ├─ clients.ts
│  ├─ changelog.ts
│  └─ projects.ts
│
├─ public/
│  ├─ products/          # product logos/screenshots (add later)
│  ├─ logos/             # client logos (SVG/PNG)
│  └─ press/
│     ├─ wallandfifth-logo.svg
│     ├─ wallandfifth-logo.png
│     └─ wallandfifth-screenshots.zip
│
├─ package.json
├─ tsconfig.json
└─ README.md
Pages
/ (Home)
Hero — product-company framing.

Products — cards from data/products.ts.

Approach — how we build.

Capabilities — AI, full-stack, data, infra.

Clients — logos/placeholders from data/clients.ts.

Changelog — public shipping log.

FAQ — timelines, pricing modes, stack.

CTA — bold action band.

Contact — mailto form (no backend).

Footer.

/products
Reuses the Products section as a full page.

/products/[slug]
Product detail if a product uses href: "/products/slug".
Status pill (Live/Beta/Incubating), tags, optional image/logo, and sections (Overview, Features, Tech, Roadmap).

/product
Redirects → /products.

/projects/[slug] (optional)
Case-study page for client/internal projects, fed by data/projects.ts.

/about
Parent-company story, operating principles, CTAs.

/press
Brand assets + “fast facts”; downloads from /public/press.

Special
app/not-found.tsx — friendly 404.

app/sitemap.ts & app/robots.ts — first-party SEO endpoints.
