

- AVFoundation
- AVMutableVideoCompositionInstruction
-  layerInstructions 

Instance Property

# layerInstructions

Instructions that specify how to layer and compose video frames from source tracks.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var layerInstructions: [AVVideoCompositionLayerInstruction] { get set }
```

## Discussion

Tracks are layered in the composition according to the top-to-bottom order of the `layerInstructions` array; the track with trackID of the first instruction in the array will be layered on top, with the track with the trackID of the second instruction immediately underneath, and so on.

If the property value is `nil`, the output is a fill of the background color.

## See Also

### Configuring the Instructions

var backgroundColor: CGColor?

The background color of the composition.

var timeRange: CMTimeRange

The time range to which the instruction applies.

var enablePostProcessing: Bool

A Boolean value that indicates whether the instruction requires post processing.

