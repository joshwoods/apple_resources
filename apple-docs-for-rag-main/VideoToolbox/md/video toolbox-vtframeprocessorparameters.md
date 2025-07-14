

- Video Toolbox
-  VTFrameProcessorParameters 

Protocol

# VTFrameProcessorParameters

The base protocol for input and output processing parameters for a frame processor implementation.

macOS 15.4+

``` source
protocol VTFrameProcessorParameters : NSObjectProtocol
```

## Overview

An instance of a class corresponding to this protocol is passed to processWithParameters:error: calls and for asynchronous versions of those calls, the same instance is returned in the completion.

## Topics

### Inspecting the parameters

var sourceFrame: VTFrameProcessorFrame

A processor frame that contains the current source frame to use for all processing features.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- VTFrameRateConversionParameters
- VTMotionBlurParameters
- VTOpticalFlowParameters

## See Also

### Frame processor

class VTFrameProcessor

A class that creates a new frame processor for the configured video effect.

class VTFrameProcessorFrame

An object that wraps video frames to send to the processor, as source, reference, or output frames.

protocol VTFrameProcessorConfiguration

A protocol that describes the configuration of a processor to use during a video processing session.

