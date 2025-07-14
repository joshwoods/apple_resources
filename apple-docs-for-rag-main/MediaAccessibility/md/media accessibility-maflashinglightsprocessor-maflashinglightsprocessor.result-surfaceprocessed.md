

- Media Accessibility
- MAFlashingLightsProcessor
- MAFlashingLightsProcessor.Result
-  surfaceProcessed 

Instance Property

# surfaceProcessed

A Boolean value that indicates whether the flashing lights processor successfully processed the input surface.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var surfaceProcessed: Bool { get }
```

## Discussion

This value is false if the flashing lights processor can’t process the surface, which can occur for unsupported hardware or unsupported color spaces.

## See Also

### Interpreting results from video processing

var intensityLevel: Float

The intensity of flashing lights in the input surface.

var mitigationLevel: Float

The amount of mitigation in the output surface.

