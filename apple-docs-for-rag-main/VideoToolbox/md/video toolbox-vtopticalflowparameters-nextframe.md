

- Video Toolbox
- VTOpticalFlowParameters
-  nextFrame 

Instance Property

# nextFrame

The next source frame in presentation time order.

macOS 15.4+

``` source
var nextFrame: VTFrameProcessorFrame { get }
```

## Discussion

This value can be set to nil for the last frame.

## See Also

### Inspecting the parameters

var sourceFrame: VTFrameProcessorFrame

The current source frame.

var destinationOpticalFlow: VTFrameProcessorOpticalFlow

A user allocated mutable optical flow that will receive the results.

var submissionMode: VTOpticalFlowParameters.SubmissionMode

A value describing the processing request in a parameters submission object.

enum SubmissionMode

A value describing the processing request in a parameters submission object.

