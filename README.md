# Laser Ops

FigUI plugin for FluidNC laser testing.

## Modes

### Focus test

Runs a set of parallel lines and lifts Z by a configured amount between each pass.

### Cut grid

Generates a grid of outline squares. Power varies across columns and speed varies across rows. No Z motion.

### Engrave grid

Generates a grid of filled squares with hatch spacing. Power varies across columns and speed varies across rows. No Z motion.

## SD export

Each mode has a `Save ... to SD` button that writes a `.nc` file under `/sd/` so you can download it later from FigUI's file manager.

## Local browser demo

Open `demo.html` through a local static server to run the plugin in a browser with an emulated SD card.

Example:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000/demo.html`.

Saved files appear in the left-hand SD panel and can be previewed or downloaded directly.

### Parameters

- Line length
- Z step
- Number of steps
- Laser power
- Feed rate
- Z feed

### Assumption

The machine is already zeroed when the plugin starts.
