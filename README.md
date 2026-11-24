# Celwerx

Celwerx is a 2D animation app that runs entirely in a web browser. It is a single HTML file with no build step and no server: open `index.html` and start drawing.

## Features

**Drawing**
- Vector drawing (editable lines and fill shapes that stay sharp at any zoom) and bitmap drawing, chosen per layer
- Brush with pen pressure and smoothing, eraser that cuts vector lines, paint bucket, line, rectangle and ellipse
- Select and transform, point editing with falloff, cutter (lasso) and a 16-point envelope warp
- Palettes with named swatches and saved brushes, with import and export

**Timeline**
- Layers with exposures and holds, drawing swaps and a per-layer drawing library
- Drag drawings to move, copy, swap or change how long they hold
- Onion skin with separate strength bars for 10 frames before and 10 after
- Timeline zoom, thin playhead, sound track with waveform and frame-by-frame scrubbing

**Animation**
- Keyframed camera (pan, zoom, rotate, easing)
- Bones with rigid or bending binding, IK, squash and stretch, weight painting
- Auto-rig from separate parts, or from one drawing by tapping the joints

**Compositing**
- Node editor with 29 node types: stack, blend, crossfade, mask, cutter, feather, color key, color adjust, levels, tint, grayscale, invert, threshold, blur, motion blur, sharpen, glow, drop shadow, outline, shade/light, fade, grain, move/scale, flip, crop, display, write and output

**App**
- File, Edit, View, Timeline, Layer and Help menus, right-click menus (long-press on touch screens), undo history with named steps
- Export the current frame as PNG, all frames as a ZIP of PNGs, or a video (MP4 or WebM depending on the browser), plus a project file you can reopen later

Press `?` in the app or use Help > Shortcuts and help for the full list of tools and keyboard shortcuts.

## Running it

**On your computer:** download `index.html` and open it in a recent version of Chrome, Edge, Firefox or Safari.

**On GitHub Pages:**
1. Push this repository to GitHub.
2. In the repository, go to Settings > Pages.
3. Under "Build and deployment", set Source to "Deploy from a branch", choose your main branch and the `/ (root)` folder, then save.
4. After a minute or two the app is live at `https://<your-username>.github.io/<repository-name>/`.

## Saving work

Projects are kept in the browser's local storage while they are small enough. That storage belongs to one browser on one device and can be cleared, so use File > Save to keep a project file (`.json`) and File > Open to load it again.

## Requirements and limits

- The image-sequence ZIP export loads the JSZip library from `cdnjs.cloudflare.com`, so it needs an internet connection. Everything else works offline.
- Video export records in real time, so keep the tab open and visible while it runs.
- Node effects, bending deformers and long scenes are heavier on phones and tablets than on desktop computers.

## License

No license has been chosen yet. Until one is added, the default copyright rules apply and others may not reuse the code. Add a `LICENSE` file once you decide how you want it shared.
