

- Compositor Services
- LayerRenderer
-  state 

Instance Property

# state

A value that indicates whether the layer renderer is currently visible and ready for you to draw content.

visionOS 1.0+

``` source
var state: LayerRenderer.State { get }
```

## Discussion

Use the state of the layer to determine when to start and stop your rendering loop. When the layer is in the LayerRenderer.State.running state, draw frames of content using your rendering loop. Stop your rendering loop when the layer enters other states. When the layer reaches the LayerRenderer.State.invalidated state, clean up and deallocate your render loop structures.

## See Also

### Managing the rendering loop

func waitUntilRunning()

Stops further execution of your code until the layer renderer leaves the paused state.

enum State

The states of the layer renderer, which tell you how to proceed with drawing operations.

struct Clock

A type that supports operations that require a precise time measurement.

