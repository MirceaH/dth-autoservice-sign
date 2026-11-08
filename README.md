# D.T.H Autoservice — 3D Wall Sign Designs

Pure HTML + CSS mock-ups of a 3D metallic wall sign for a family-run car service
(**D.T.H** on the first line, **AUTOSERVICE** right-aligned below it, the "A" starting
under the "H").

No framework, no build step, no JavaScript needed for the look itself — the metallic
effect is built from layered CSS gradients (`background-clip: text`) and stacked
`drop-shadow` filters.

## Pages

| File | What it shows |
|------|---------------|
| [`index.html`](index.html) | Main design on a textured wall, with 4 colourways you can switch between: **Gold**, **Chrome**, **Red**, **Copper** |
| [`variants.html`](variants.html) | 6 different lettering styles / fonts: Futuristic (Orbitron), Classic Gold (Bebas Neue), Military (Black Ops One), Retro Bold (Bungee), Stencil Cut (Saira Stencil One), Sport Garage (Russo One) |

## Techniques

- Metallic text via multi-stop `linear-gradient` + `background-clip: text`
- Depth via chained `drop-shadow()` filters (hard offset shadows for the retro style)
- Wall texture from repeating gradients + an inline SVG `feTurbulence` noise layer
- Responsive sizing with `clamp()` and `aspect-ratio`
- Staggered entrance animation with `@keyframes` and `animation-delay`
- `variants.html` drives all six looks from CSS custom properties, so a new style is
  one block of variables

## Run it

Open `index.html` or `variants.html` in any browser (Google Fonts are loaded from the web).
