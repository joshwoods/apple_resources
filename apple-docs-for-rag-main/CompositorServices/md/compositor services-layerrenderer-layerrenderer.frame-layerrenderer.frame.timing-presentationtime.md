

- Compositor Services
- LayerRenderer
- LayerRenderer.Frame
- LayerRenderer.Frame.Timing
-  presentationTime 

Instance Property

# presentationTime

The time at which the system displays the frame onscreen.

visionOS 1.0+

``` source
var presentationTime: LayerRenderer.Clock.Instant { get }
```

## Discussion

You can use the presentation time as a synchronization point for other parts of your app. For example, if you play an audio clip when the frame appears, configure your code to start playing the clip at the specified time.

