

- Compositor Services
- LayerRenderer
-  waitUntilRunning() 

Instance Method

# waitUntilRunning()

Stops further execution of your code until the layer renderer leaves the paused state.

visionOS 1.0+

``` source
func waitUntilRunning()
```

## Discussion

Call this function to let the system handle events while you wait for the layer to become ready. The function services incoming layer-related events until the layer exits the paused state.

## See Also

### Managing the rendering loop

var state: LayerRenderer.State

A value that indicates whether the layer renderer is currently visible and ready for you to draw content.

enum State

The states of the layer renderer, which tell you how to proceed with drawing operations.

struct Clock

A type that supports operations that require a precise time measurement.

