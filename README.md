# Servo Bench

**A free, real-size 3D servo simulator that runs in your browser.** Snap hobby servos together, turn their horns, and see how your robot arm or linkage moves *before* you buy or wire a single part.

**▶ Try it live:** https://python736.github.io/servo-bench/

<!-- Add a screenshot: save one as screenshot.png in this folder, then remove the comment marks below. -->
<!-- ![Servo Bench screenshot](screenshot.png) -->

## Features

- **Real dimensions:** SG90, MG90S and MG996R servos, modelled from datasheet sizes in millimetres.
- **Drag-and-drop building:** drop a servo on an orange dot to plug it onto another servo's arm or body. Pull it away to unplug it.
- **Free movement:** move with arrows, rotate with rings (5° snapping, hold Shift for free rotation), or type exact values.
- **Realistic motion:** each servo turns at its rated speed and shows the estimated load from the servos it carries.
- **Horn and link options:** single, double and cross horns, links of any length, and custom colors.
- **Ray tracing (optional):** path-traced lighting similar to Blender Cycles. It refines only when nothing moves and throttles itself on slower PCs.
- **Motion steps:** save poses as steps and press Play to watch your build run through them at real servo speed.
- **Arduino code export:** get a ready-to-upload sketch for Arduino Uno/Nano/Mega or ESP32, with pin choices, smooth synchronised moves, and timing taken from each servo's rated speed. Copy it or download it as a `.ino` file.
- **Parts list:** see every part you need (servos, links, brackets, board, power supply), with shop links.
- **Saves automatically** in your browser. You can also export and import builds as text.

## Controls

| Action | How |
|---|---|
| Move a servo | Drag it, or use the arrows (**W**) |
| Rotate a servo | Rings (**E**), or **R** to turn 90° and **T** to tip it over |
| Turn the shaft | Drag the white horn |
| Nudge | Arrow keys, PageUp / PageDown |
| Ray tracing | **L** |
| Remove | **Delete** |
| Camera | Drag empty space to orbit, right-drag to pan, scroll to zoom |

## Run it locally

No install or build step is needed. Open `index.html` in Chrome, Edge or Firefox.

It loads [three.js](https://threejs.org) from a CDN, so it needs an internet connection the first time.

## Built with

- [three.js](https://github.com/mrdoob/three.js) (MIT)
- [three-gpu-pathtracer](https://github.com/gkjohnson/three-gpu-pathtracer) (MIT)
- [three-mesh-bvh](https://github.com/gkjohnson/three-mesh-bvh) (MIT)

## Support

Servo Bench is free and ad-free. If it helped you, press the ❤ **Support** button in the app, star this repo, or share it with a friend.

**Maintainers:** donation buttons and the Amazon affiliate tag are set in the `window.SERVO_BENCH` block near the end of `index.html`. A service only shows up once you fill in its username.

## License

[MIT](LICENSE): free to use, change and share, including commercially.
