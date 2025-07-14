

- Compositor Services
-  CompositorFrameIndex 

Type Alias

# CompositorFrameIndex

The sequential index for a frame in the compositor’s timeline.

visionOS 1.0+

``` source
typealias CompositorFrameIndex = UInt64
```

## Discussion

During the creation of your content, the compositor creates frames for you to render your content. This type stores the index the compositor assigns to that frame. The compositor presents frames sequentially based on their indexes.

## See Also

### Getting frame-related details

var frameIndex: LayerFrameIndex

The sequential index number of a frame.

typealias LayerFrameIndex

A frame index in the layer’s timeline.

