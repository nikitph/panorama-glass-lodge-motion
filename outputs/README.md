# Panorama Glass Lodge — motion study

An 18-second square, silent animation derived from the supplied website screenshot.

## Technique

- Website components are separated into independently animated layers.
- Architectural geometry, fine rules, typography and interface shapes are authored as SVG.
- Photographs stay raster images, framed through SVG viewports. Wrapping a photograph in SVG does not make it vector artwork.
- A deterministic GSAP timeline controls motion and HyperFrames renders the video.

The original source is 500 × 500 pixels. The render has a 1080 × 1080 canvas, with sharp vector elements; it cannot recover missing photographic detail.

The source package contains the editable HTML composition and local assets. Use `npx hyperframes preview --background` from its folder to open the timeline; use `npx hyperframes render --quality delivery --output panorama.mp4` to render.
