

- Compositor Services
- LayerRenderer
- LayerRenderer.Drawable
-  presentationFrameIndex 

Instance Property

# presentationFrameIndex

The sequential index of a drawable’s frame.

visionOS 1.0+

``` source
var presentationFrameIndex: CompositorFrameIndex { get }
```

## Discussion

When your immersive space becomes visible, you start drawing frames of content. Compositor Services assigns a sequential index to each frame to indicate its position in the final output. You can use these indexes to differentiate frames during drawing or predict future frame indexes. For example, you might start playback of an audio file when a specific frame appears.

## See Also

### Synchronizing the drawing operation

var frameTiming: LayerRenderer.Frame.Timing

The timing information for the drawable’s frame.

