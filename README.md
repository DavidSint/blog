# David Sint's Blog

This repo uses the Astro framework and is based on the template blog.

- ✅ 100/100 Lighthouse performance
- ✅ SEO-friendly with canonical URLs and OpenGraph data
- ✅ Sitemap support
- ✅ RSS Feed support
- ✅ Markdown & MDX support

## 🚀 Project Structure

Inside of this Astro project, there is the following folders and files:

```text
├── public/
├── src/
│   ├── components/
│   ├── content/
│   ├── layouts/
│   └── pages/
├── astro.config.mjs
├── README.md
├── package.json
└── tsconfig.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

There's nothing special about `src/components/`, but that's where the Astro/React/Vue/Svelte/Preact components reside.

The `src/content/` directory contains ["collections"](https://docs.astro.build/en/guides/content-collections/) of related Markdown and MDX documents. `getCollection()` is used to retrieve posts from `src/content/blog/`, and type-check the frontmatter using the schema.

Any static assets, like images, are placed in the `public/` directory.

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |
| `npm run format:fix`      | Run the Biome formatter to write fixes           |
| `npm run linter:fix`      | Run the Biome linter to write fixes              |
| `npm run check:fix`       | Run the Biome formatter & linter to write fixes  |

## Credit

This theme is based off of the [Astro Blog template](https://github.com/withastro/astro/tree/latest/examples/blog) which is based off of [Bear Blog](https://github.com/HermanMartinus/bearblog/).
