

- Video Toolbox
- VTOpticalFlowParameters
-  VTOpticalFlowParameters.SubmissionMode 

Enumeration

# VTOpticalFlowParameters.SubmissionMode

A value describing the processing request in a parameters submission object.

macOS 15.4+

``` source
enum SubmissionMode
```

## Topics

### Enumeration Cases

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

var nextFrame: VTFrameProcessorFrame

The next source frame in presentation time order.

var destinationOpticalFlow: VTFrameProcessorOpticalFlow

A user allocated mutable optical flow that will receive the results.

var submissionMode: VTOpticalFlowParameters.SubmissionMode

A value describing the processing request in a parameters submission object.

