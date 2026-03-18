# AGENTS.md

## Architecture Overview
This is a static website built with Astro for Hekwerkmeesters, a fencing company. The site uses a single `Layout.astro` for consistent navigation, footer, and global styles. Pages are located in `src/pages/` and render static content without dynamic data fetching.

## Key Patterns
- **Page Structure**: Each page imports `Layout.astro`, defines frontmatter for title/description, and includes inline `<style>` blocks for page-specific CSS. Example: `src/pages/diensten.astro` uses frontmatter arrays for service data and inline styles for layout.
- **Styling**: Global CSS variables (e.g., `--gold`, `--black-deep`) defined in `Layout.astro` for consistent theming. Inline styles per page avoid global conflicts.
- **Navigation**: Active link highlighting based on `Astro.url.pathname` in `Layout.astro`.
- **Content**: Dutch language throughout; static text and images from `/public/`.

## Developer Workflows
- **Development**: Run `npm run dev` for local server at `localhost:4321`.
- **Build**: Use `npm run build` to generate production files in `./dist/`.
- **Preview**: Test builds with `npm run preview`.
- **Node Version**: Requires Node.js >=22.12.0 as specified in `package.json`.

## Conventions
- **File Naming**: Pages use lowercase with hyphens (e.g., `over-ons.astro`).
- **Images**: Stored in `/public/` and referenced with absolute paths (e.g., `/hero_bg.jpeg`).
- **No External Integrations**: Pure Astro setup without databases or APIs.

## Key Files
- `src/layouts/Layout.astro`: Defines CSS variables, navbar, footer, and mobile menu script.
- `src/pages/index.astro`: Homepage with hero, about, and services sections.
- `src/pages/diensten.astro`: Services page with data array in frontmatter for dynamic rendering.</content>
<parameter name="filePath">/home/kevin/WebstormProjects/hekwerkmeesters/AGENTS.md
