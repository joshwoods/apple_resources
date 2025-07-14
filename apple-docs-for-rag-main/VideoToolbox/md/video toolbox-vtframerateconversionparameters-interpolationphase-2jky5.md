

- Video Toolbox
- VTFrameRateConversionParameters
-  interpolationPhase 

Instance Property

# interpolationPhase

An array of floating-point values that indicate which intervals to insert a frame between the current and next frame.

macOS 15.4+

``` source
var interpolationPhase: [Float] { get }
```

## Discussion

Array size indicates how many frames are needed to interpolate and needs to match destinationFrames array size, where there is one interval for each destination frame. Float number values should be between 0 and 1, e.g. to insert one frame in the middle, a value of 0.5 can be used.

## See Also

### Inspecting the parameters

var sourceFrame: VTFrameProcessorFrame

The current source frame.

var nextFrame: VTFrameProcessorFrame?

The next source frame in presentation time order.

var opticalFlow: VTFrameProcessorOpticalFlow?

A property that defines the optical flow for an object.

var submissionMode: VTFrameRateConversionParameters.SubmissionMode

A value describing the processing request in a parameters submission object.

enum SubmissionMode

A value describing the processing request in a parameters submission object.

var destinationFrames: [VTFrameProcessorFrame]

A caller-allocated array of frames that contains the pixel buffers to receive the results.

