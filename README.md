# portfolio-neue

Personal portfolio site: Home, About, and Projects. Built with Astro.

## Stack

- Astro + TypeScript
- React (`@astrojs/react`) for interactive islands such as the theme toggle
- MDX content collections for project write-ups
- Tailwind CSS

## Commands

| Command           | Action                                      |
| ----------------- | ------------------------------------------- |
| `npm install`     | Install dependencies                        |
| `npm run dev`     | Start the local dev server                  |
| `npm run build`   | Build the static site to `./dist/`          |
| `npm run preview` | Preview the production build locally        |

## Adding a project

1. Duplicate `src/content/projects/example-project.mdx`.
2. Update the frontmatter (`title`, `description`, `date`, optional `tags`, `image`, `link`).
3. Replace the MDX body with the write-up.

## Adding a blog later

Create `src/content/blog/config.ts` (same pattern as projects) and register it in `src/content.config.ts`. No other restructuring is required.

## Deploy

This is a static Astro site. Connect the GitHub repo to Vercel; no extra adapter or GitHub Actions workflow is included.
