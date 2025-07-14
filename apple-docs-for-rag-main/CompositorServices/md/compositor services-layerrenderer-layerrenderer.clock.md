

- Compositor Services
- LayerRenderer
-  LayerRenderer.Clock 

Structure

# LayerRenderer.Clock

A type that supports operations that require a precise time measurement.

visionOS 1.0+

``` source
struct Clock
```

## Overview

Use this type to perform time-related operations during the rendering of a frame. For example, call wait(until:tolerance:) to pause your render loop until the optimal rendering time arrives.

## Topics

### Putting the current thread to sleep

func wait(until: LayerRenderer.Clock.Instant, tolerance: Duration?)

Blocks the current thread until the specified time.

### Creating a clock

init()

Creates a new clock type.

## Relationships

### Conforms To

- Clock
- Copyable
- Sendable

## See Also

### Managing the rendering loop

var state: LayerRenderer.State

A value that indicates whether the layer renderer is currently visible and ready for you to draw content.

func waitUntilRunning()

Stops further execution of your code until the layer renderer leaves the paused state.

enum State

The states of the layer renderer, which tell you how to proceed with drawing operations.

