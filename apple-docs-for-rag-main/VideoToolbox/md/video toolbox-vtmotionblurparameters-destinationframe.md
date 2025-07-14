

- Video Toolbox
- VTMotionBlurParameters
-  destinationFrame 

Instance Property

# destinationFrame

A user-allocated pixel buffer that receives the results.

macOS 15.4+

``` source
var destinationFrame: VTFrameProcessorFrame { get }
```

## See Also

### Inspecting the parameters

var sourceFrame: VTFrameProcessorFrame

The current source frame.

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

