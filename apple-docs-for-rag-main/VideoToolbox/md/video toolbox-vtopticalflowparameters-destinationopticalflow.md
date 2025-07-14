

- Video Toolbox
- VTOpticalFlowParameters
-  destinationOpticalFlow 

Instance Property

# destinationOpticalFlow

A user allocated mutable optical flow that will receive the results.

macOS 15.4+

``` source
var destinationOpticalFlow: VTFrameProcessorOpticalFlow { get }
```

## See Also

### Inspecting the parameters

var sourceFrame: VTFrameProcessorFrame

The current source frame.

var nextFrame: VTFrameProcessorFrame

The next source frame in presentation time order.

var submissionMode: VTOpticalFlowParameters.SubmissionMode

A value describing the processing request in a parameters submission object.

enum SubmissionMode

A value describing the processing request in a parameters submission object.

