

- Video Toolbox
- VTFrameRateConversionParameters
-  nextFrame 

Instance Property

# nextFrame

The next source frame in presentation time order.

macOS 15.4+

``` source
var nextFrame: VTFrameProcessorFrame? { get }
```

## Discussion

For the last frame this value will be nil.

## See Also

### Inspecting the parameters

var sourceFrame: VTFrameProcessorFrame

The current source frame.

var opticalFlow: VTFrameProcessorOpticalFlow?

A property that defines the optical flow for an object.

var interpolationPhase: [Float]

An array of floating-point values that indicate which intervals to insert a frame between the current and next frame.

var submissionMode: VTFrameRateConversionParameters.SubmissionMode

A value describing the processing request in a parameters submission object.

enum SubmissionMode

A value describing the processing request in a parameters submission object.

var destinationFrames: [VTFrameProcessorFrame]

A caller-allocated array of frames that contains the pixel buffers to receive the results.

