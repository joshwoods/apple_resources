

- Video Toolbox
- VTFrameRateConversionParameters
-  VTFrameRateConversionParameters.SubmissionMode 

Enumeration

# VTFrameRateConversionParameters.SubmissionMode

A value describing the processing request in a parameters submission object.

macOS 15.4+

``` source
enum SubmissionMode
```

## Overview

Set to VTFrameRateConversionParametersSubmissionModeSequential to indicate that the current submission follows the presentation time order without jumping or skipping when compared to the previous submission. Using the submission mode sequential will yield better performance. Set to VTFrameRateConversionParametersSubmissionModeRandom to indicate a skip or a jump in frame sequence. If the submission mode random is set, the internal cache will be cleared during the processWithParameters call.

## Topics

### Submission modes

case random

A submission follow presentation time order with a jump or skip in a frame sequence.

case sequential

A submission follow presentation time order without a jump or skip when compared to a previous submission.

### Initializers

init?(rawValue: Int)

### Enumeration Cases

case sequentialReferencesUnchanged

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

var nextFrame: VTFrameProcessorFrame?

The next source frame in presentation time order.

var opticalFlow: VTFrameProcessorOpticalFlow?

A property that defines the optical flow for an object.

var interpolationPhase: [Float]

An array of floating-point values that indicate which intervals to insert a frame between the current and next frame.

var submissionMode: VTFrameRateConversionParameters.SubmissionMode

A value describing the processing request in a parameters submission object.

var destinationFrames: [VTFrameProcessorFrame]

A caller-allocated array of frames that contains the pixel buffers to receive the results.

