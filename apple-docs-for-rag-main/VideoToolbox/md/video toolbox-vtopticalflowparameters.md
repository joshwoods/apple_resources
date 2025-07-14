

- Video Toolbox
-  VTOpticalFlowParameters 

Class

# VTOpticalFlowParameters

An object that describes frame-level optical flow parameters.

macOS 15.4+

``` source
class VTOpticalFlowParameters
```

## Topics

### Creating a parameters object

init?(sourceFrame: VTFrameProcessorFrame, nextFrame: VTFrameProcessorFrame, submissionMode: VTOpticalFlowParameters.SubmissionMode, destinationOpticalFlow: VTFrameProcessorOpticalFlow)

### Inspecting the parameters

var sourceFrame: VTFrameProcessorFrame

The current source frame.

var nextFrame: VTFrameProcessorFrame

The next source frame in presentation time order.

var destinationOpticalFlow: VTFrameProcessorOpticalFlow

A user allocated mutable optical flow that will receive the results.

var submissionMode: VTOpticalFlowParameters.SubmissionMode

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

### Optical flow

class VTFrameProcessorOpticalFlow

A class to wrap bidirectional optical flow to send to the processor.

class VTOpticalFlowConfiguration

A configuration object that enables optical flow on a frame processing session.

