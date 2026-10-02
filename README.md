# Our World

An interactive loop about scale, and about how much one small life holds. Click through it from the edge of the observable universe, to a paper earth pinned on a wall, to the room inside "you", out to the whole planet, the moon, the pale blue dot, and back to the galaxies again.

**Live:** [mpts.ie/games/ourworld](https://mpts.ie/games/ourworld/)

After [a reel by @sopaguada](https://www.tiktok.com/@sopaguada/video/7690600273236004103) on TikTok.

![The Hubble eXtreme Deep Field, the opening screen](docs/screenshots/01-galaxy.jpg)

## The loop

### 1. The galaxies

The Hubble eXtreme Deep Field, resting in a soft black vignette. Click anywhere and a sharp black pinhole closes on a single galaxy.

![A black pinhole closing on one galaxy](docs/screenshots/02-pinhole.jpg)

### 2. The wall

The pinhole opens onto a wall: a child's pencil drawing of the earth, cut out of paper and pinned up, beside five polaroids (a dune, a butterfly, a glacier, two hands almost touching, a sunset). In the corner: *this is all we have*.

![A paper earth and five polaroids pinned to a wall](docs/screenshots/03-wall.jpg)

Everything here is 3D. The pushpins are modelled pins that cast shadows onto the photos and the wall. Pull a pin and its photo lets go of the wall: it drops, hooks up to one side in a **J**, then rocks side to side in smile-shaped **C** arcs, bending and rippling like cloth, with a gleam sliding across the print as it tilts. You can grab a falling photo and pull it back up; it only starts falling again.

![A polaroid coming loose and fluttering down](docs/screenshots/04-polaroid-falls.jpg)

Take out the pin holding the earth and the whole wall comes down with it, the lowest photo first, each one above it a moment later.

![The earth and the photos falling from the wall](docs/screenshots/05-wall-comes-down.jpg)

### 3. Inside "you"

Underneath is the room inside "you": an orange halftone field, a 1px line that wanders without end (it bulges softly away from your cursor and you can drag it), and four words that switch on like an old CRT: *me*, *my worries*, *my fears*, *my life*.

![The room inside you](docs/screenshots/06-inside-you.jpg)

Hover a word and the letter under the cursor grows while the word breaks into heavy VHS glitching.

![A word glitching under the cursor](docs/screenshots/07-glitch.jpg)

Press Esc (or click the paper) and the room winds down: the words switch off, the line burns away like a wick, the dots recede, and the page folds into a small square on the globe.

### 4. That's a whole planet

A 3D earth with exaggerated relief, lit from the upper left and fading softly into the dark on its night side. Drag to spin it and fling it to send it turning. Pencil-style callouts appear one at a time over real places on land: *just had a child*, *mother just died*, *just had breakfast*… Click the "you" square to go back inside.

![The globe with callouts](docs/screenshots/08-whole-planet.jpg)

### 5. From the moon

Click empty space and the camera pulls back onto a cratered lunar horizon, with a box around the earth: *everybody who has ever lived*. You can keep spinning the earth here, and all the way through the moves on either side.

![The earth above the lunar horizon](docs/screenshots/09-earthrise.jpg)

Click again and you lift off the moon, swing round until it slips behind the earth, and draw back until the earth is a single bright point.

![The moon and the earth in the same frame](docs/screenshots/10-orbit.jpg)

### 6. The pale blue dot

That point becomes Voyager 1's pale blue dot, suspended in a pillar of scattered light, and a line types itself out beside it.

![The pale blue dot with the words maybe you should worry less](docs/screenshots/11-pale-blue-dot.jpg)

Click once more and the dot becomes the galaxy you first fell into, which grows until it fills the screen, and the loop begins again.

![The galaxies growing back out of the dot](docs/screenshots/12-back-to-the-galaxies.jpg)

## Controls

| Where | What you can do |
|---|---|
| Galaxies | Click or press Space to go in |
| Wall | Click a pin to drop its photo; grab and pull photos; take out the earth's pin (or press Space) to go on |
| Inside "you" | Push and drag the line; hover the words; Esc, Space or a click on the paper to zoom out |
| Globe | Drag and fling to spin; scroll to zoom; click "you" to go back in; click empty space (or Space) to go to the moon |
| Moon and orbit | Drag and fling to spin the earth; click or Space to go on |
| Pale blue dot | Click or Space to return to the galaxies |

## Credits

- **Inspiration:** [a reel by @sopaguada](https://www.tiktok.com/@sopaguada/video/7690600273236004103) on TikTok.
- **Hubble eXtreme Deep Field (2012):** NASA, ESA, G. Illingworth, D. Magee, P. Oesch (UC Santa Cruz), R. Bouwens (Leiden) and the HUDF09 team.
- **Pale Blue Dot Revisited (PIA23645, 2020):** NASA/JPL-Caltech, from Voyager 1's 1990 image. The pillar of light around the dot is a reworking of that image.
- **Earth texture and elevation:** NASA Blue Marble and NASA elevation data.
- **The polaroid photographs and the paper earth** were generated for this project.
- Built with [three.js](https://threejs.org/), Archivo Narrow and VT323 from Google Fonts.

## Development

The site is static: everything lives in [`public/games/ourworld/`](public/games/ourworld/) (one `index.html` and its images). A small Cloudflare Worker serves it at `mpts.ie/games/ourworld` and redirects the bare path to the trailing-slash URL.

```bash
npm install
npm run dev      # local preview
npm run deploy   # deploy the worker and its assets
```
