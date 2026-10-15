# FeelCanvas — Devpost write-up

## Elevator pitch

Type how you feel. Watch it become art. FeelCanvas turns any feeling into
generative art — and teaches you color theory along the way.

## Inspiration

Most people can say "I feel bad" but not *which* bad — and art classes teach
color theory with paint swatches, not feelings. FeelCanvas connects the two:
your emotion becomes the input, and a unique artwork becomes the output.
It is a tool for expression first, and a lesson second — you learn why warm
golds feel hopeful and deep blues feel heavy by seeing your own feelings
painted in them.

## What it does

Pick one of 8 feelings — Joy, Calm, Sadness, Anger, Love, Anxiety, Hope,
Nostalgia — or type your own ("stressed" maps to Anxiety, "happy" to Joy).
FeelCanvas draws a unique procedural artwork for that feeling: sunburst rays
for Joy, layered waves for Calm, falling rain for Sadness, jagged shards for
Anger, blooms and hearts for Love, tangled lines for Anxiety, a rising
sunrise for Hope, sepia film grain for Nostalgia. Every piece comes with a
plain-English explanation of the color psychology behind it. Regenerate for a
new variation, download any piece as a PNG wallpaper, or browse the gallery
of all 8 feelings.

## How we built it

Single-file HTML + CSS + vanilla JavaScript, drawing on the Canvas API.
Each emotion has a small painter function with its own palette and motif,
driven by a seeded random generator (mulberry32) so artworks are unique yet
reproducible. No AI key, no server, no downloaded images — every shape,
gradient, grain speck, and vignette is computed live in the browser.

## Challenges we ran into

The hardest part was making eight feelings feel *distinct* with code alone.
Early versions of Anxiety and Sadness looked alike — both dark and messy —
so we gave Anxiety jittery looping lines (thoughts that never settle) and
Sadness steady vertical rain (quiet and constant). The second challenge was
honesty in the keyword mapping: instead of pretending to understand any
word, unknown feelings map to the closest feeling with a note that says so.

## Accomplishments that we're proud of

A tool that is genuinely two things at once: an art generator anyone can
enjoy in ten seconds, and a color-theory lesson that sticks because it is
about *your* feelings, not a textbook swatch.

## What we learned

Color theory is not abstract — it is emotional. People remember that "blue
means calm" when they have just watched their own calm become waves. Teaching
through feeling beats teaching through definitions.

## What's next for FeelCanvas

More feelings (awe, boredom, courage), a "share your feeling" gallery, and a
classroom mode where teachers can use it to start conversations about
emotions and art.

## Built with

HTML, CSS, JavaScript, Canvas API
