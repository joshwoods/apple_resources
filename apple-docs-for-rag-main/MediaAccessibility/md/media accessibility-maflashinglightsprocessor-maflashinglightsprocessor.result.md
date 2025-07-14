

- Media Accessibility
- MAFlashingLightsProcessor
-  MAFlashingLightsProcessor.Result 

Structure

# MAFlashingLightsProcessor.Result

An object that reports the result of the flashing lights processor.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct Result
```

## Overview

An MAFlashingLightsProcessor.Result object is the result of calling processSurface(_:outSurface:timestamp:options:). This object indicates whether the method successfully processed the input surface, the intensity of flashing lights in the input surface, and the amount of mitigation in the output surface.

## Topics

### Interpreting results from video processing

var surfaceProcessed: Bool

A Boolean value that indicates whether the flashing lights processor successfully processed the input surface.

var intensityLevel: Float

The intensity of flashing lights in the input surface.

var mitigationLevel: Float

The amount of mitigation in the output surface.

## See Also

### Processing video content

func processSurface(IOSurfaceRef, outSurface: inout IOSurfaceRef, timestamp: CFAbsoluteTime, options: [MAFlashingLightsProcessor.OptionKey : Any]?) -> MAFlashingLightsProcessor.Result

Processes a surface by analyzing pixels for sequences of flashing lights and mitigates them by dimming the content.

struct OptionKey

Options for the flashing lights processor.

