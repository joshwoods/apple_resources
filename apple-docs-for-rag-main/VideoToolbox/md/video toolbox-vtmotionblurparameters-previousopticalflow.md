

- Video Toolbox
- VTMotionBlurParameters
-  previousOpticalFlow 

Instance Property

# previousOpticalFlow

Optional optical flow object that contains forward and backward optical flow with the previous frame.

macOS 15.4+

``` source
var previousOpticalFlow: VTFrameProcessorOpticalFlow? { get }
```

## Discussion

For the first frame this will always be nil. This object is only needed if optical flow is pre-computed.

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

var submissionMode: VTMotionBlurParameters.SubmissionMode

A value describing the processing request in a parameters submission object.

enum SubmissionMode

A value describing the processing request in a parameters submission object.

