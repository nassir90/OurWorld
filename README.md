# Our World

ThreeJS conversion of [a video about the solar system](https://www.tiktok.com/@sopaguada/video/7690600273236004103) by @sopaguada.

**Live:** [mpts.ie/games/ourworld](https://mpts.ie/games/ourworld/)

![Galaxies](docs/screenshots/01-galaxy.jpg)

![Pinhole](docs/screenshots/02-pinhole.jpg)

![Wall](docs/screenshots/03-wall.jpg)

![Polaroid falling](docs/screenshots/04-polaroid-falls.jpg)

![Wall coming down](docs/screenshots/05-wall-comes-down.jpg)

![Inside "you"](docs/screenshots/06-inside-you.jpg)

![Glitch](docs/screenshots/07-glitch.jpg)

![Globe](docs/screenshots/08-whole-planet.jpg)

![Moon](docs/screenshots/09-earthrise.jpg)

![Orbit](docs/screenshots/10-orbit.jpg)

![Pale blue dot](docs/screenshots/11-pale-blue-dot.jpg)

![Back to the galaxies](docs/screenshots/12-back-to-the-galaxies.jpg)

## Credits

- **Original reel:** [@sopaguada](https://www.tiktok.com/@sopaguada/video/7690600273236004103) on TikTok.
- **Hubble eXtreme Deep Field (2012):** NASA, ESA, G. Illingworth, D. Magee, P. Oesch (UC Santa Cruz), R. Bouwens (Leiden) and the HUDF09 team.
- **Pale Blue Dot Revisited (PIA23645, 2020):** NASA/JPL-Caltech, from Voyager 1's 1990 image. The pillar of light around the dot is a reworking of that image.
- **Earth texture and elevation:** NASA Blue Marble and NASA elevation data.
- **The polaroid photographs and the paper earth** were generated for this project.
- Built with [three.js](https://threejs.org/), Archivo Narrow and VT323 from Google Fonts.

## License

The code is [MIT](LICENSE). The NASA and ESA imagery keeps the terms credited above.

## Development

Static site in [`public/games/ourworld/`](public/games/ourworld/), served at `mpts.ie/games/ourworld` by a Cloudflare Worker.

```bash
npm install
npm run dev      # local preview
npm run deploy   # deploy the worker and its assets
```
