# Astroblast

A pocket planetarium: a live map of the real night sky above you, right in your
browser. Drag to pan, pinch to zoom, or point your phone at the sky.

**Live page:** https://maridizzle.github.io/astroblast/ (once GitHub Pages is enabled)

## Features

- Real-time positions of about 9,000 stars, colored by their true surface temperature
- Constellation figures, the naked-eye planets, and the Moon with its current phase
- Set any location by GPS, city, or latitude and longitude, and any date and time
- Adjustable star limit and label brightness, matching astroterm's options
- Live weather for your spot (temperature, cloud cover, wind, sunrise and sunset),
  with an optional overlay that dims the star field by how cloudy it is
- Point-at-sky mode that follows where you aim your phone, with calibration arrows
- Works on phones and desktops and remembers your settings on each device

## How it works

Star positions come from the Yale Bright Star Catalog. Constellation figures come
from Stellarium. Planet and Moon positions are computed from NASA JPL orbital
elements. All of the astronomy math is ported to JavaScript from the open-source
[astroterm](https://github.com/da-luce/astroterm) project. Weather comes from
[Open-Meteo](https://open-meteo.com).

Everything runs in a single self-contained HTML file. There is no build step and
no server.

## Hosting

This is a static page served with GitHub Pages from the `main` branch (root).
Point-at-sky and live weather need an https address, which Pages provides. Opening
`index.html` straight from disk will show the stars but not those two features.

## Credits

- Stars: Yale Bright Star Catalog (Harvard)
- Constellation figures: Stellarium, by way of astroterm
- Planet and Moon orbits: NASA Jet Propulsion Laboratory
- Weather: Open-Meteo
- Astronomy code ported from astroterm (MIT licensed)

Made by Maridizzle.
