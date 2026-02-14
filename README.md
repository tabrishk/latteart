# Latte Flow Mobile MVP

Mobile web prototype for latte-art practice with touch-first controls and optional device tilt.

## What is included

- Touch pour simulation on a cup canvas
- Vertical flow slider (pour rate)
- Tap-to-cut-through gesture
- Optional device tilt for cup angle drift
- Shape lessons: Dot, Heart, Tulip, Rosetta, Swan
- Live score against a target mask

## Run locally

From `/Users/david/Documents/latte`:

```bash
python3 -m http.server 8080 --bind 0.0.0.0
```

Then open:

- On this machine: `http://localhost:8080`
- On phone (same Wi-Fi): `http://<YOUR_COMPUTER_IP>:8080`

To find your computer IP on macOS:

```bash
ipconfig getifaddr en0
```

(if empty, try `en1`)

## Mobile test notes

- Use Safari (iOS) or Chrome (Android)
- On iOS, tilt needs a user tap on `Enable Tilt` to request permission
- Best used in landscape orientation

## Controls

- Drag finger: pour path
- Right slider: pour flow rate
- Quick tap on cup: cut-through
- Enable Tilt: toggle cup-tilt emulation
- Reset Cup: clear liquid surface
- Prev/Next Shape: switch tutorial target
