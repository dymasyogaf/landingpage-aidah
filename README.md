# Aidah Landing Page

Landing page untuk [aidah.web.id](https://aidah.web.id) — Asisten keuangan pribadi berbasis AI.

Built with **Astro** + **Cloudflare Pages**.

## 🏗️ Struktur Proyek

```
├── public/              # Static assets (favicon, images)
├── src/
│   ├── components/      # Astro components
│   │   ├── Navbar.astro
│   │   ├── Hero.astro
│   │   ├── Features.astro
│   │   ├── HowItWorks.astro
│   │   ├── Testimonials.astro
│   │   ├── CallToAction.astro
│   │   ├── Footer.astro
│   │   └── ScrollReveal.astro
│   ├── layouts/
│   │   └── Layout.astro  # Base layout + global styles
│   └── pages/
│       └── index.astro   # Landing page
├── astro.config.mjs      # Astro config with Cloudflare adapter
├── package.json
└── tsconfig.json
```

## 🚀 Development

```bash
npm install
npm run dev
```

Dev server berjalan di `http://localhost:4321`

## 📦 Build

```bash
npm run build
```

Output di folder `dist/`.

## ☁️ Deploy ke Cloudflare Pages

### Via Dashboard:
1. Push repo ke GitHub
2. Buka [Cloudflare Pages](https://dash.cloudflare.com/) → **Workers & Pages** → **Create**
3. Connect ke repository GitHub
4. Settings:
   - **Build command**: `npm run build`
   - **Build output directory**: `dist`
   - **Framework preset**: Astro
5. Klik **Save and Deploy**

### Via Wrangler CLI:
```bash
npx wrangler pages deploy dist
```
