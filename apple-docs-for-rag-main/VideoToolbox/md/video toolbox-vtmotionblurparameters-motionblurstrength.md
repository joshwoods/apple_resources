

- Video Toolbox
- VTMotionBlurParameters
-  motionBlurStrength 

Instance Property

# motionBlurStrength

A value that indicates the strength of blur to apply.

macOS 15.4+

``` source
var motionBlurStrength: Int { get }
```

## Discussion

The supported range for this value is from 1 and 100. The default value is 50.

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

var nextOpticalFlow: VTFrameProcessorOpticalFlow?

Optional optical flow object that contains forward and backward optical flow with the next frame.

var previousOpticalFlow: VTFrameProcessorOpticalFlow?

Optional optical flow object that contains forward and backward optical flow with the previous frame.

var submissionMode: VTMotionBlurParameters.SubmissionMode

A value describing the processing request in a parameters submission object.

enum SubmissionMode

A value describing the processing request in a parameters submission object.

