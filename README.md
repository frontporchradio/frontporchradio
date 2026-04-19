# Front Porch Radio

> _The only radio station playing music made by us....for us._

A single-page, static, zero-build website for Front Porch Radio — an independent community station spinning Americana, folk, blues, and soul.

## What's in this repo

```
.
├── index.html     # The entire site — HTML, CSS, JS, and SVG art in one file
├── logo.svg       # Brand logo (scalable, used by nav/hero/footer/favicon)
├── logo.png       # Optional raster fallback (drop one in if you want)
├── README.md      # You are here
├── LICENSE        # MIT
└── .gitignore
```

**Logo:** `logo.svg` is included and wired into four places — nav bar, hero,
footer, and favicon. It's a hand-drawn, scalable recreation of the Front
Porch Radio shield (gold badge, green "Front Porch" banner, farm-scene oval,
vintage microphone, cursive "Radio" script, and brown ribbon with the
domain). If you'd prefer a raster version, drop a `logo.png` (transparent
background, ~1024×1024) alongside `logo.svg` and the site will use the PNG as
a fallback if the SVG ever fails to load. If both are missing, the site falls
back to a generated porch illustration automatically.

There is no build step. No bundler, no framework, no npm install. Open `index.html` in any browser and the site runs.

## Features

- Warm, responsive front-porch Americana aesthetic (Fraunces serif + Inter sans)
- Hand-drawn SVG illustration: porch ceiling, railing with 22 balusters, perspective floor slats, two rocking chairs, a vintage tabletop radio, and a layered cornfield view at sunset with a distant barn
- Sticky navigation with "Listen Live" call-to-action and a pulsing on-air indicator
- "Now Playing" bar with rotating demo tracks
- Day-tabbed weekly schedule with an auto-highlighted live slot for the current time
- Show grid, hosts section, "Our Story," Listen Anywhere platform tiles
- Newsletter signup (front-end only — wire to a real service when ready)
- Dark-forest footer with social links

## Local development

```bash
# Option A: just open the file
open index.html           # macOS
xdg-open index.html       # Linux
start index.html          # Windows

# Option B: serve locally (recommended for consistent font loading)
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploying

Because this is a single static file, you have lots of options:

**GitHub Pages** — push this repo to GitHub, go to **Settings → Pages**, set source to `main` branch, `/` root. Site will be live at `https://<username>.github.io/<repo>` within a minute.

**Namecheap Shared Hosting (cPanel)** — upload `index.html` to `public_html/` via File Manager or FTP.

**Namecheap EasyWP** — this is a static site, not WordPress. You'd either install it as a custom theme or switch to regular shared hosting.

**Netlify / Vercel / Cloudflare Pages** — connect the repo and deploy. Zero config needed.

## What's a placeholder

- DJ names, show names, and bios are invented. Swap for the real ones.
- Listen Live / play buttons are visual only — when you have a stream URL, wire them to a real `<audio>` element.
- Newsletter signup just fires a front-end confirmation. Connect to Mailchimp, Buttondown, ConvertKit, etc.
- Social links in the footer point to `#`. Fill in real URLs.

## License

MIT — see [LICENSE](./LICENSE). Feel free to use and adapt.
