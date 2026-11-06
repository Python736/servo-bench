# Contributing to Servo Bench

Thanks for wanting to help! Servo Bench is a single HTML file with no build step, so getting started takes seconds.

## Run it

1. Fork and clone the repo.
2. Open `index.html` in Chrome, Edge or Firefox, or serve the folder with any static server (for example `npx serve .`).
3. Edit, save, refresh.

Useful link options while testing:

| Option | Effect |
|---|---|
| `?example=arm3` | Open an example (`start`, `arm3`, `b2b`, `scara`) |
| `?theme=light` / `?theme=dark` | Force a theme |
| `?quality=low` / `?quality=high` | Force the graphics tier |
| `?tips=0` | Hide the tips card |

## Where things live in `index.html`

| Look for | What it is |
|---|---|
| `const TYPES` | Servo models with datasheet sizes, speed and torque. **Adding a servo starts here** |
| `const PRESETS` | Example builds |
| `function buildServo` | The 3D model of a servo |
| `function renderFrame` | Drawing and adaptive resolution |
| `function buildSketch` | Arduino / ESP32 code export |
| `function partsRows` | Parts list |
| `window.SERVO_BENCH` | Site settings: links, donation usernames |

## Good first contributions

- **A new servo model** (DS3218, MG92B, continuous rotation): add an entry to `TYPES` with datasheet dimensions in mm.
- **New example builds** in `PRESETS`.
- **Code export targets**, such as a PCA9685 16-channel driver.

## Pull requests

- Keep each pull request focused on one thing.
- Test with a normal and a large build, and in light and dark themes.
- Keep it fast: the app must run smoothly on laptops with built-in graphics.

Questions? Open a [discussion](https://github.com/Python736/servo-bench/discussions).
