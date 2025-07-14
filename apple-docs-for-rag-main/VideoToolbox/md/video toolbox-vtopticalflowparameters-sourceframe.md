

- Video Toolbox
- VTOpticalFlowParameters
-  sourceFrame 

Instance Property

# sourceFrame

The current source frame.

macOS 15.4+

``` source
var sourceFrame: VTFrameProcessorFrame { get }
```

## Discussion

This must be a non-nil value.

## See Also

### Inspecting the parameters

var nextFrame: VTFrameProcessorFrame

The next source frame in presentation time order.

var destinationOpticalFlow: VTFrameProcessorOpticalFlow

A user allocated mutable optical flow that will receive the results.

var submissionMode: VTOpticalFlowParameters.SubmissionMode

A value describing the processing request in a parameters submission object.

enum SubmissionMode

A value describing the processing request in a parameters submission object.

