

- Video Toolbox
- VTMotionBlurParameters
-  submissionMode 

Instance Property

# submissionMode

A value describing the processing request in a parameters submission object.

macOS 15.4+

``` source
var submissionMode: VTMotionBlurParameters.SubmissionMode { get }
```

## Discussion

Set to VTMotionBlurParametersSubmissionModeSequential to indicate that the current submission follows the presentation time order without jumping or skipping when compared to the previous submission. Using the submission mode sequential will yield better performance. Set to VTMotionBlurParametersSubmissionModeRandom to indicate a skip or a jump in frame sequence. If submission mode random is set, the internal cache will be cleared during the processWithParameters call.

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

var previousOpticalFlow: VTFrameProcessorOpticalFlow?

Optional optical flow object that contains forward and backward optical flow with the previous frame.

enum SubmissionMode

A value describing the processing request in a parameters submission object.

