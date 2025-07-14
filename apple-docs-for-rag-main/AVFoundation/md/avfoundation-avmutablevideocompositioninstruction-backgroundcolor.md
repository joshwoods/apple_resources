

- AVFoundation
- AVMutableVideoCompositionInstruction
-  backgroundColor 

Instance Property

# backgroundColor

The background color of the composition.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var backgroundColor: CGColor? { get set }
```

## Discussion

Only solid BGRA colors are supported; patterns and other supported colors are ignored. If the rendered pixel buffer does not have alpha, the alpha value of the background color is ignored.

If the background color is `NULL`, the video compositor uses a default background color of opaque black.

## See Also

### Configuring the Instructions

var layerInstructions: [AVVideoCompositionLayerInstruction]

Instructions that specify how to layer and compose video frames from source tracks.

var timeRange: CMTimeRange

The time range to which the instruction applies.

var enablePostProcessing: Bool

A Boolean value that indicates whether the instruction requires post processing.

