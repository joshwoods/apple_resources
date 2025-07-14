

- Compositor Services
- LayerRenderer
- LayerRenderer.Frame
-  frameIndex 

Instance Property

# frameIndex

The sequential index number of a frame.

visionOS 1.0+

``` source
var frameIndex: LayerFrameIndex { get }
```

## Discussion

The layer assigns a unique index number to each frame, starting at the first frame and incrementing the index by `1` for each new frame.

## See Also

### Getting frame-related details

typealias LayerFrameIndex

A frame index in the layer’s timeline.

typealias CompositorFrameIndex

The sequential index for a frame in the compositor’s timeline.

