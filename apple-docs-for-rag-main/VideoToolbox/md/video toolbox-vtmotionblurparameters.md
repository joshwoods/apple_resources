

- Video Toolbox
-  VTMotionBlurParameters 

Class

# VTMotionBlurParameters

This object contains both input and output parameters necessary to run the motion blur processor on a frame.

macOS 15.4+

``` source
class VTMotionBlurParameters
```

## Overview

This object is used in the processWithParameters call of the VTFrameProcessor class. The output parameter is a destinationFrame where the output frame is returned as a VTFrameProcessorFrame back to the caller function once processWithParameters completes.

The parameters within VTMotionBlurParameters are frame level parameters.

## Topics

### Creating a parameters object

init?(sourceFrame: VTFrameProcessorFrame, nextFrame: VTFrameProcessorFrame?, previousFrame: VTFrameProcessorFrame?, nextOpticalFlow: VTFrameProcessorOpticalFlow?, previousOpticalFlow: VTFrameProcessorOpticalFlow?, motionBlurStrength: Int, submissionMode: VTMotionBlurParameters.SubmissionMode, destinationFrame: VTFrameProcessorFrame)

### Inspecting the parameters

var sourceFrame: VTFrameProcessorFrame

The current source frame.

var destinationFrame: VTFrameProcessorFrame

A user-allocated pixel buffer that receives the results.

var nextFrame: VTFrameProcessorFrame?

The next source frame in presentation time order.

var previousFrame: VTFrameProcessorFrame?

The previous source frame in presentation time order.

var motionBlurStrength: Int

A value that indicates the strength of blur to apply.

var nextOpticalFlow: VTFrameProcessorOpticalFlow?

Optional optical flow object that contains forward and backward optical flow with the next frame.

var previousOpticalFlow: VTFrameProcessorOpticalFlow?

Optional optical flow object that contains forward and backward optical flow with the previous frame.

var submissionMode: VTMotionBlurParameters.SubmissionMode

A value describing the processing request in a parameters submission object.

enum SubmissionMode

A value describing the processing request in a parameters submission object.

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

### Motion blur

class VTMotionBlurConfiguration

A configuration object to enable motion blur on a frame processing session.

