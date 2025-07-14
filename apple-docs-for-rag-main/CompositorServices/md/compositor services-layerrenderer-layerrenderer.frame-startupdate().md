

- Compositor Services
- LayerRenderer
- LayerRenderer.Frame
-  startUpdate() 

Instance Method

# startUpdate()

Notifies Compositor Services that you started updating the app-specific content for the frame.

visionOS 1.0+

``` source
func startUpdate()
```

## Mentioned in 

Drawing fully immersive content using Metal

## Discussion

This function helps you optimize your app’s rendering efficiency. Before you render a frame, you might need to respond to interactions with your content and update your app’s data structures before you render items in your scene. Call this function immediately before you start that work, and call endUpdate() as soon as you finish. Compositor Services uses the time difference to improve its predictions for when to start the frame encoding process.

Move as much work as possible into the update phase to minimize encoding time. Don’t do any work that relies on the current pose information during the update phase. Instead, make any pose-related changes during the submission phase.

## See Also

### Reporting frame update times

func endUpdate()

Notifies Compositor Services that you finished updating the app-specific content you need to render the frame.

