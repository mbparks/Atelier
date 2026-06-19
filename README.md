# ATELIER

Field Instrument No. 035. A preparatory bench for the painter. Version 0.5.0.

ATELIER is the whole pre-paint stage in one instrument. Everything you work out
before a brush touches the surface: the design (value), the bones (structure and
perspective), and the color (key, harmony, mixing). It is built around a single
shared document, the reference image plus the canvas ratio plus the working
palette plus the focal marker, so each family enriches the others rather than
standing alone.

## Families

ATELIER is organized into four families that map to what the artist actually does.

- See. Reductions that reveal the design. A value mode (notan, 2 to 5 steps,
  squint, value bias), a warm and cool temperature mode, a Sobel edge mode, and a
  color key that lifts the dominant notes from the reference.
- Build. Construction that imposes the bones. The aspect aware armature (thirds,
  golden section, dynamic symmetry with the eyes of the rectangle, rabatment,
  golden spiral, center cross, nodes), the crop and format explorer with root
  rectangle formats, the transfer grid with real world scaling math, and a one,
  two, or three point perspective grid.
- Color. The harmony wheel (complement, analogous, triad, split, tetrad), the
  Gurney gamut mask, and the Kubelka-Munk mixing bench with a curated pigment
  core of twenty nine pigments. The color key from See feeds in as match targets.
- Check. Flip and mirror, the value mass centroid, the caliper for angle and
  proportion sighting, the focal readout, and the small multiples notan ladder.

## Build status

All five phases are installed.

- Phase 1, foundation. Shell, module and tab chrome, shared document state, value
  scale ruler, composite plate export. Done.
- Phase 2, See and Build core. Notan value reduction and the aspect aware
  armature. Done.
- Phase 3, reductions and construction. Temperature map, edge map, color key,
  crop and format explorer, root rectangle formats, transfer grid, perspective.
  Done.
- Phase 4, the Color family. Harmony wheel, gamut mask, Kubelka-Munk mixing bench.
  Done.
- Phase 5, the Check family and polish. Flip, value mass, caliper, focal readout,
  small multiples, about panel, focus styles, reduced motion, responsive layout.
  Done.

## Use

Open the file in any modern browser. Mount a reference by clicking Mount or by
dragging an image onto the bench, or lay a blank ground to plan a composition from
scratch. Choose a format, reduce to value under See, lay an armature under Build,
plan the palette under Color, and verify under Check. Click the plate to drop a
focal marker. Export writes a composite PNG of the current plate with the active
overlays baked in.

## Notes on the methods

- Mixing uses single constant Kubelka-Munk in the red, green, and blue channels.
  This is the standard inexpensive subtractive model. It is an approximation of
  full spectral mixing, but it behaves the way paint does. Blue and yellow give a
  muddy green rather than a flat gray, white lightens, and complements neutralize.
- Temperature uses a hue based warm and cool split with a neutral band threshold,
  so low saturation areas read as neutral mass rather than forced warm or cool.
- The golden spiral is drawn as a true logarithmic spiral around the golden eye,
  scaled to fill the plate, so it reads as a clean compositional guide.
- The value mass centroid is weighted by darkness, so it reports where the dark
  mass sits relative to true center.

## Conventions

Single file HTML, no build step, no server dependencies. Dark default. Vintage
scientific instrument aesthetic. No em dashes anywhere in prose or code. The
reference never leaves the browser, all processing is local.

## License

GPL-3.0

This program is free software: you can redistribute it and/or modify it under the
terms of the GNU General Public License as published by the Free Software
Foundation, either version 3 of the License, or any later version. This program is
distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY, without
even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
See the GNU General Public License for more details.
