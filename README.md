# FORM / LAB

A lightweight image playground with ASCII, ordered dithering, halftone, particles, and pin art. Upload an image or use a camera, adjust the controls, and export a PNG.

## Run locally

No dependencies or build step are required. With Python 3 installed, run from this directory:

```sh
python3 -m http.server 8765 --bind 127.0.0.1
```

Open http://localhost:8765 and allow camera access if you want to use live input. Camera requires localhost or HTTPS.

## Features

- ASCII character sets and color controls
- Ordered dithering and halftone dots
- Motion-driven particles with return to their original positions
- Pin art with adjustable height and tilt
- Optional empty-background capture for camera pin impressions
- PNG export at 960 × 720

Image and camera processing stays in the browser. There are no external libraries, model downloads, API keys, or backend services.

Pin art creates a stylized impression; it does not measure physical depth. For clearer camera impressions, keep the camera still, capture an empty background, then step into frame.

## Files

- `index.html`: interface
- `style.css`: design system and responsive layout
- `app.js`: image processing, camera input, animation, and export

Deploy these three files to any static host using HTTPS.
