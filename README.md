# Lafiya — deployable site

Single-file static site. No build step, no dependencies.

## Run locally
Open `index.html` in a browser, or serve the folder:

    npx serve .

## Deploy (any of these, about two minutes)
- **Netlify**: drag this folder onto https://app.netlify.com/drop
- **Vercel**: `npx vercel` inside this folder
- **GitHub Pages**: push the folder to a repo, Settings → Pages → deploy from branch
- **Cloudflare Pages**: create a project, upload the folder

## Media
Photos load from Unsplash and video from Mixkit (both free licences, see CREDITS.md).
All media URLs live in one object near the top of the `<script>` block:

    const MEDIA = { heroPoster: {...}, heroVideo: {...}, ... }

To self-host (recommended before the final submission, so the demo never depends on a third-party CDN):
1. Download each file from the page URL listed in CREDITS.md.
2. Put them in `assets/` and change the `src` values to `assets/<file>`.
3. For the hero video, download the HD version from the Mixkit page; the bundled link is the 360p preview.

Set `MEDIA_ON = false` to show the gradient panels instead of media (useful for a slow connection demo).

## Languages
All interface strings are in the `T` object (`en`, `yo`, `ha`, `ig`). Yorùbá, Hausa and Igbo
translations need a native-speaker review before submission.

## Emergency steps
Written from standard first-aid guidance. Have a clinician or Red Cross trainer sign them off.
