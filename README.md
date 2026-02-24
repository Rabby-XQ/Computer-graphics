# 3D Rotation Visualizer

An interactive single-file HTML demo for understanding **3D rotation transformations** around the X, Y, and Z axes.

## What this project does

This visualizer renders a wireframe cube on a canvas and shows how it rotates in real time around a selected axis.

It includes:
- Axis selection: **X**, **Y**, or **Z**
- Real-time animation with adjustable speed
- Manual angle control using a slider
- Play/Pause toggle
- Reset angle to `0°`
- Rotation formulas that update with the selected axis
- Live coordinate output for a sample point `(1, 1, 0)` after rotation
- Visual helpers: grid, 3D axes, highlighted active axis, rotation arc, ghost/trail cubes

## Controls

- **X — AXIS ROTATION**: Rotate around X-axis
- **Y — AXIS ROTATION**: Rotate around Y-axis
- **Z — AXIS ROTATION**: Rotate around Z-axis
- **SPEED** slider: Changes auto-rotation speed (`0` to `5`, step `0.5`)
- **ANGLE** slider: Manually set angle (`0°` to `360°`) and pauses auto-play
- **PLAY / PAUSE** button: Start or stop animation
- **RESET** button: Set angle back to `0°`

## Rotation equations shown in UI

### Around X-axis
- `x' = x`
- `y' = y cosθ − z sinθ`
- `z' = y sinθ + z cosθ`

### Around Y-axis
- `x' = x cosθ + z sinθ`
- `y' = y`
- `z' = z cosθ − x sinθ`

### Around Z-axis
- `x' = x cosθ − y sinθ`
- `y' = x sinθ + y cosθ`
- `z' = z`

## How to run

No build tools or dependencies are required.

1. Open `3d-rotation.html` in any modern browser.
2. Interact with the control panel to explore 3D rotation behavior.

## File structure

- `3d-rotation.html` — Full app (HTML, CSS, and JavaScript in one file)
