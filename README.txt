# Chandan Samanta — Ultron Portfolio (3D / cinematic)

## Run it
1. Extract the folder.
2. Open `index.html` in Chrome, Edge or Firefox (double-click works; no server or internet needed —
   Three.js is bundled in `vendor/`). Use VS Code "Live Server" if you prefer.

## What's inside
- `index.html`   page structure
- `styles.css`   black & white premium theme with red / deep-blue / purple accents, 3D cards, responsive
- `scene.js`     WebGL scene: Ultron head that follows the pointer, camera flight through a glowing
                 tunnel as you scroll, light colours that shift per section, shockwave on click
- `script.js`    custom cursor + glow trail, 3D tilt/spotlight cards, magnetic buttons, skill sphere,
                 timeline, certificate filter + document viewer
- `data.js`      ALL your content — experience, projects, skills, certificates, honours
- `assets/`      portrait.jpg, signature.png, resume.pdf,
                 certificates/ (original documents), previews/ (images shown on the page)
- `vendor/three.min.js`  Three.js r128 (local copy)

## Fonts
Headings use **Algerian**, body text uses **Times New Roman** (both are Windows/Office system fonts).
Devices without Algerian (Mac, Linux, most phones) fall back to Cinzel (loaded from Google Fonts when online),
then Times New Roman. The hero name auto-fits so Algerian's wide letters never overflow.

## Editing
- Add a certificate: drop the file into `assets/certificates/`, save a preview image (JPG) in
  `assets/previews/`, then add one line to `CERTS` in `data.js`.
- Add an experience / project / skill: add an entry to `EXPERIENCE`, `PROJECTS` or `SKILLS` in `data.js`.
- Experience cards link to their certificates through the `certs: [...]` ids.

## Notes
- Contact links open email / social profiles; there is no server-side form.
- Your phone number from the résumé is intentionally NOT shown on the page. The résumé PDF itself is linked.
- Project cards describe the work from your READMEs. GitHub links go to your profile (individual repo URLs were not supplied).
- Respects "reduce motion" settings; the custom cursor is disabled on touch devices.
