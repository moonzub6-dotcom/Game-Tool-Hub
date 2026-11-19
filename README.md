# GameToolHub

A dark, responsive gaming-tools website built with Astro. It includes working starter tools for Minecraft and a clearly labelled Palworld breeding planner.

## Included
- Homepage and game directory pages
- Palworld: breeding planner (manual planning worksheet; does not claim to calculate official breeding outcomes)
- Palworld: type matchup reference calculator (editable matchup assumptions in `src/scripts/tools.js`)
- Minecraft: Nether coordinate converter
- Minecraft: XP level calculator
- Minecraft: small crafting recipe helper
- About, Contact, Privacy Policy and Terms pages
- `robots.txt` and `sitemap.xml`

## Run locally
1. Install Node.js (LTS).
2. Extract this ZIP.
3. Open a terminal in this folder.
4. Run `npm install`
5. Run `npm run dev`
6. Open the local URL printed by Astro.

## Deploy to Cloudflare Pages with GitHub
1. Create a GitHub repository named `gametoolhub`.
2. Upload/extract the contents of this folder into the repository root (the `package.json` must be at the root).
3. In Cloudflare Dashboard, open Workers & Pages → Create → Pages → Connect to Git.
4. Select the `gametoolhub` repository.
5. Framework preset: Astro. Build command: `npm run build`. Build output directory: `dist`.
6. Deploy. Cloudflare will provide a `*.pages.dev` address.
7. If the Pages project already exists and is currently deployed from manual uploads, connect Git only after checking the current production deployment and keeping a backup. Do not delete the existing project.

## Important
- Replace the placeholder contact email in `src/pages/contact.astro` before launch.
- Update `site` in `astro.config.mjs` if the final Pages hostname differs.
- The sitemap is a static starter sitemap. Keep it aligned with published pages if you add/remove routes.
- Palworld breeding outcomes are game-data dependent and can change with updates. The included planner is a manual planning worksheet, not an authoritative breeding-result engine. Add a verified, versioned dataset before advertising exact offspring predictions.
- Review all game names, logos and images before launch. GameToolHub is an independent fan-made tools site and is not affiliated with Mojang or Pocketpair.
