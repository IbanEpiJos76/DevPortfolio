### 📁 Directory Structure
```
├── public/              # Global static assets (placeholder.jpg, favicon)
├── src/
│   ├── assets/          # Project & Profile images (Supports automatic Astro optimization)
│   ├── components/      # Reusable Astro components
│   ├── data/            # JSON files for project data
│   ├── layouts/         # Layout templates with Meta tags
│   ├── pages/           # Site routes (index.astro)
│   └── styles/          # Global CSS styles
│   └── config.ts        # Global site configuration
├── astro.config.mjs     # Astro configuration
└── tsconfig.json        # TypeScript configuration
```

### 🔍 SEO & AI Optimization
All SEO and AI metadata is driven from `src/data/home.json`. Update the fields below to improve search engine, social media and AI crawler visibility:

| Field | Description |
| :------------ | :----------------------------------------------------------- |
| `siteUrl` | Your deployed domain (e.g. `https://yourname.dev`). Required for canonical URLs, sitemap and absolute OG image links. |
| `webpageTitle` | Page tab title and Open Graph title tag. |
| `description` | Primary intro summary used for meta description, Open Graph, Twitter preview cards and `/llms.txt`. |
| `lang` | Page language code (e.g. `en`, `fr`, `de`). Sets the `<html lang>` attribute. |
| `jobTitle` | Your role — included in JSON-LD structured data shown to search engines and `/llms.txt`. |
| `keywords` | Comma-separated keywords for the `<meta name="keywords">` tag. |
| `twitterHandle` | Your Twitter/X username (with or without `@`). Enables Twitter Card attribution. |
| `ogImageUrl` | Path to your Open Graph preview image. Use a **1200×630 px** image for best results across all platforms. |

> **Automatic Features:**
> - `sitemap-index.xml` & `robots.txt`: Auto-generated at build time.
> - `/llms.txt`: Dynamically generated Markdown portfolio route for AI agents and LLM web crawlers (powered by [`src/pages/llms.txt.ts`](file:///Users/nabil/_projects/astro-trial/career-portfolio-template/src/pages/llms.txt.ts)).



### 📚 Useful commands and links for reference:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

Tailwind CSS: `npx astro add tailwind`

Inter font: `npm install @fontsource-variable/inter` 

Space Grotesk font: `npm install @fontsource-variable/space-grotesk`

Astro-icon: `npx astro add astro-icon`

Material Desing Icons: `npm install @iconify-json/mdi`

https://docs.astro.build/en/guides/styling/#add-tailwind-4

https://www.astroicon.dev

https://icon-sets.iconify.design/mdi/?category=Material

## 🤝 Contributing
Contributions are welcome!  
Please read the [Contributing Guide](CONTRIBUTING.md) before opening a PR.

## 📝 License
This project is licensed under the [MIT License](LICENSE)
