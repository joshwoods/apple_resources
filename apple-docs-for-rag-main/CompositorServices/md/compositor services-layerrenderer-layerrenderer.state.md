

- Compositor Services
- LayerRenderer
-  LayerRenderer.State 

Enumeration

# LayerRenderer.State

The states of the layer renderer, which tell you how to proceed with drawing operations.

visionOS 1.0+

``` source
enum State
```

## Topics

### Getting the states

case paused

A state that indicates the layer is paused and not currently drawing.

case running

A state that indicates the layer is visible and ready for you to draw your content.

case invalidated

A state that indicates the layer no longer supports drawing operations.

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing the rendering loop

var state: LayerRenderer.State

A value that indicates whether the layer renderer is currently visible and ready for you to draw content.

func waitUntilRunning()

Stops further execution of your code until the layer renderer leaves the paused state.

struct Clock

A type that supports operations that require a precise time measurement.

