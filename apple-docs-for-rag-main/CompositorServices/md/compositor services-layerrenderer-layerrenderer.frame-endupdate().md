

- Compositor Services
- LayerRenderer
- LayerRenderer.Frame
-  endUpdate() 

Instance Method

# endUpdate()

Notifies Compositor Services that you finished updating the app-specific content you need to render the frame.

visionOS 1.0+

``` source
func endUpdate()
```

## Mentioned in 

Drawing fully immersive content using Metal

## Discussion

This function helps you optimize your app’s rendering efficiency. Before you render a frame, you might need to respond to interactions and update your app’s data structures before you render items in your scene. Call startUpdate() immediately before you start that work, and call this function as soon as you finish. Compositor Services uses the frame update time to improve its predictions for when to start the frame encoding process.

Move as much work as possible into the update phase to minimize encoding time. Don’t do any work that relies on the current pose information during the update phase. Instead, make any pose-related changes during the submission phase.

## See Also

### Reporting frame update times

func startUpdate()

Notifies Compositor Services that you started updating the app-specific content for the frame.

