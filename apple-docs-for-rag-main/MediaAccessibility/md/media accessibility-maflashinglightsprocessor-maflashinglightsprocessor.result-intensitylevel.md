

- Media Accessibility
- MAFlashingLightsProcessor
- MAFlashingLightsProcessor.Result
-  intensityLevel 

Instance Property

# intensityLevel

The intensity of flashing lights in the input surface.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var intensityLevel: Float { get }
```

## Discussion

The result is a value between `0` and `100`, where `100` is the highest detectable intensity for flashing lights.

## See Also

### Interpreting results from video processing

var surfaceProcessed: Bool

A Boolean value that indicates whether the flashing lights processor successfully processed the input surface.

var mitigationLevel: Float

The amount of mitigation in the output surface.

