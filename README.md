# RetroArch Overlays

Custom RetroArch overlay files for TrimUI devices (Smart Pro, Brick). Only GBA for now.

![Example](docs/example.jpeg)

> ^ `tsp-gba-grid` overlay

- `(device)-gba`: Only GBA logo
- `(device)-gba-grid`: GBA logo and pixel grid (similar to lcd1x shader)
- `(device)-gba-grid-narrow`: GBA logo and pixel grid with narrower lines. Pixels are wider, less accurate to original hardware.

## Using

1. `Quick Menu -> On-Screen Overlay`: Set `Overlay Preset` to a `.cfg` file in this repository
2. `Settings -> Video -> Scaling`:
	1. Enable `Integer Scale` (Balanced pixels, ensures screen is correctly sized for the overlay)
	2. Set `Viewport Anchor Bias Y` to `0.00` (Positions the screen to the top to give space for the GBA logo)

## Editing

The source `(device)-gba.af` files are available in the `src` directory if you want to adjust things like grid and GBA logo opacity. Just export to a PNG matching the filename you want to update, or you can name it something else, then duplicate one of the `.cfg` files and edit it to point to the new `.png` file you created.

## TODO

- [x] TrimUI Brick
- [ ] Other systems
