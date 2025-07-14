

- Video Toolbox
-  VTFrameRateConversionParameters 

Class

# VTFrameRateConversionParameters

An object that contains the required input and output parameters to run a frame rate conversion processor on a frame.

macOS 15.4+

``` source
class VTFrameRateConversionParameters
```

## Overview

This object is used in the processWithParameters call of a VTFrameProcessor class. The output parameter is a destinationFrame where the output frame is returned as a VTFrameProcessorMutableFrame back to the caller function once the processing completes.

The parameters within VTFrameRateConversionParameters are frame level parameters.

## Topics

### Creating conversion parameters

convenience init?(sourceFrame: VTFrameProcessorFrame, nextFrame: VTFrameProcessorFrame, opticalFlow: VTFrameProcessorOpticalFlow?, interpolationPhase: [Float], submissionMode: VTFrameRateConversionParameters.SubmissionMode, destinationFrames: [VTFrameProcessorFrame])

Creates a new frame rate conversion parameters object.

### Inspecting the parameters

var sourceFrame: VTFrameProcessorFrame

The current source frame.

var nextFrame: VTFrameProcessorFrame?

The next source frame in presentation time order.

var opticalFlow: VTFrameProcessorOpticalFlow?

A property that defines the optical flow for an object.

var interpolationPhase: [Float]

An array of floating-point values that indicate which intervals to insert a frame between the current and next frame.

var submissionMode: VTFrameRateConversionParameters.SubmissionMode

A value describing the processing request in a parameters submission object.

enum SubmissionMode

A value describing the processing request in a parameters submission object.

var destinationFrames: [VTFrameProcessorFrame]

A caller-allocated array of frames that contains the pixel buffers to receive the results.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- VTFrameProcessorParameters

## See Also

### Frame rate conversion

class VTFrameRateConversionConfiguration

An object that enables the frame rate conversion on a frame processing session.

