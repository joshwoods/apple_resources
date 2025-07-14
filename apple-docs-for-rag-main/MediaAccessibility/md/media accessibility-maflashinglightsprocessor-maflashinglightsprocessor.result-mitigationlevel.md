

- Media Accessibility
- MAFlashingLightsProcessor
- MAFlashingLightsProcessor.Result
-  mitigationLevel 

Instance Property

# mitigationLevel

The amount of mitigation in the output surface.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var mitigationLevel: Float { get }
```

## Discussion

The result is a value between `0` and `100`, where `100` is the highest level of mitigation that can apply to the output surface, indicating the output is completely dark.

## See Also

### Interpreting results from video processing

var surfaceProcessed: Bool

A Boolean value that indicates whether the flashing lights processor successfully processed the input surface.

var intensityLevel: Float

The intensity of flashing lights in the input surface.

