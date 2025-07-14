

- Video Toolbox
- VTOpticalFlowParameters
-  submissionMode 

Instance Property

# submissionMode

A value describing the processing request in a parameters submission object.

macOS 15.4+

``` source
var submissionMode: VTOpticalFlowParameters.SubmissionMode { get }
```

## See Also

### Inspecting the parameters

var sourceFrame: VTFrameProcessorFrame

The current source frame.

var nextFrame: VTFrameProcessorFrame

The next source frame in presentation time order.

var destinationOpticalFlow: VTFrameProcessorOpticalFlow

A user allocated mutable optical flow that will receive the results.

enum SubmissionMode

A value describing the processing request in a parameters submission object.

