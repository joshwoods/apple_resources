

- Video Toolbox
- VTMotionBlurParameters
-  VTMotionBlurParameters.SubmissionMode 

Enumeration

# VTMotionBlurParameters.SubmissionMode

A value describing the processing request in a parameters submission object.

macOS 15.4+

``` source
enum SubmissionMode
```

## Overview

Set to VTMotionBlurParametersSubmissionModeSequential to indicate that the current submission follows the presentation time order without jumping or skipping when compared to the previous submission. Using the submission mode sequential will yield better performance. Set to VTMotionBlurParametersSubmissionModeRandom to indicate a skip or a jump in frame sequence. If the submission mode random is set, the internal cache will be cleared during the processWithParameters call.

## Topics

### Submission modes

case random

A submission follow presentation time order with a jump or skip in a frame sequence.

case sequential

A submission follow presentation time order without a jump or skip when compared to a previous submission.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

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

