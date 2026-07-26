# Laser Ops

FigUI plugin for FluidNC laser testing.

## Modes

### Focus test

Runs a set of parallel lines and lifts Z by a configured amount between each pass.

### Cut grid

Generates a grid of outline squares. Power varies across columns and speed varies across rows.

### Engrave grid

Generates a grid of filled squares with hatch spacing. Power varies across columns and speed varies across rows.

### Parameters

- Line length
- Z step
- Number of steps
- Laser power
- Feed rate
- Z feed
- Safe Z

### Assumption

The machine is already zeroed when the plugin starts.
