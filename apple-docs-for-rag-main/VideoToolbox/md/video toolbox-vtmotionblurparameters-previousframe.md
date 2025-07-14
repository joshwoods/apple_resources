

- Video Toolbox
- VTMotionBlurParameters
-  previousFrame 

Instance Property

# previousFrame

The previous source frame in presentation time order.

macOS 15.4+

``` source
var previousFrame: VTFrameProcessorFrame? { get }
```

## Discussion

This value can be set to nil for the first frame.

## See Also

### Inspecting the parameters

var sourceFrame: VTFrameProcessorFrame

The current source frame.

var destinationFrame: VTFrameProcessorFrame

A user-allocated pixel buffer that receives the results.

var nextFrame: VTFrameProcessorFrame?

The next source frame in presentation time order.

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

