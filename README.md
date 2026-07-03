# rm.rar portfolio v2 — closer to itzCrih's layout

## What changed from v1
- Two-column hero (avatar/bio/links on the left, a "featured" panel on the right — itzCrih puts a video there; yours is a placeholder box until you have an edit to feature)
- Particle background (same particles.js library itzCrih uses)
- Font Awesome icons instead of the colored logo icons
- Footer with columns like itzCrih's (Links / Explore)
- A "Platforms" stats section with dashes instead of made-up numbers — fill in real counts once you have them, don't leave fake numbers up

## Uploading (same as before — all files in repo root, no subfolder)
Upload index.html and avatar.png to your existing repo (drag onto the file list page, or click "Add file" → "Upload files"), commit, and Pages will rebuild automatically in a minute or two.

## About the broken avatar in your screenshot
If your avatar showed as a broken image before, it's almost always one of these:
1. The file didn't actually get committed — check your repo's file list on github.com and confirm `avatar.png` is listed at the root (not missing, not inside a folder).
2. Filename case mismatch — GitHub is case-sensitive. The file must be exactly `avatar.png` (all lowercase) and the HTML must reference it exactly the same way. This version already matches.
3. Browser cache — do a hard refresh (Ctrl+Shift+R / Cmd+Shift+R) on your live site after uploading.

## Editing content
- Bio: search for `<div class="bio">`
- Links: search for `<div class="links-grid">`
- Projects/Edits/Platforms cards: search for `id="projects"`, `id="edits"`, `id="platforms"`
- Accent color: change `--accent` near the top of the `<style>` block
