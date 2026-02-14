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

## Controls (Phone as Pitcher)

- `Enable Pitcher`: requests sensor permission and enables motion controls
- `Calibrate Grip`: sets current hold angle as neutral pitcher position
- Tilt phone forward/back: controls pour flow
- Roll phone left/right: controls horizontal drawing path
- `Flip Roll`: invert left-right direction if your device reports opposite
- `Flip Pour`: invert forward-back pour direction if needed
- Vertical slider: assist gain (how strongly tilt affects flow)
- Down-up-down motion during pours: gives rhythm bonus to score
- `Reset Cup`: clear liquid surface
- `Prev/Next Shape`: switch tutorial target
- `Start Tutorial`: auto-animates near-perfect motion and result for the current shape
- `Stop Tutorial`: returns to normal pitcher practice mode
