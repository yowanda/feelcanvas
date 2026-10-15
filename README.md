# FeelCanvas — Type how you feel. Watch it become art.

Pick a feeling — or type your own — and FeelCanvas turns it into generative
art. Eight emotions, eight distinct palettes and motifs, each with a
plain-English explanation of the color psychology behind it. Built for the
InnovArt 2027 hackathon (Art + Technology).

## What it does

- **8 feelings:** Joy, Calm, Sadness, Anger, Love, Anxiety, Hope, Nostalgia —
  each with its own palette and motif (Joy = sunburst rays, Calm = layered
  waves, Sadness = falling rain, Anger = jagged shards, Love = blooms and
  hearts, Anxiety = tangled lines, Hope = sunrise, Nostalgia = sepia + film
  grain).
- **Type a feeling:** "stressed" maps to Anxiety, "happy" to Joy, and so on.
  Unknown words map to the closest feeling (Calm) with an honest note.
- **Regenerate:** a new seeded variation of the same feeling.
- **Download PNG:** save the artwork as a wallpaper.
- **Gallery of all 8:** mini-canvases for every feeling; tap one to make it
  the hero artwork.
- **Learn:** every piece comes with 2–3 sentences on *why* those colors and
  shapes — a small lesson in color theory with every artwork.

## How the generative art works

Every artwork is drawn procedurally on the HTML `<canvas>` by a small
painter function per emotion. A seeded random generator (mulberry32) makes
each piece unique but reproducible: the same seed always draws the same
artwork. No AI key, no server, no images downloaded — all shapes, gradients,
grain, and vignettes are computed in the browser.

## Run it

Open `index.html` in any browser. Zero install, no build step, no backend.

## Live demo

https://yowanda.github.io/feelcanvas/

## Privacy

Nothing leaves the browser. No tracking, no account, no uploads.
