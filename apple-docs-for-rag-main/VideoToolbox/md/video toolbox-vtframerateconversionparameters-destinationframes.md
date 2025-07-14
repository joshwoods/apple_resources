

- Video Toolbox
- VTFrameRateConversionParameters
-  destinationFrames 

Instance Property

# destinationFrames

A caller-allocated array of frames that contains the pixel buffers to receive the results.

macOS 15.4+

``` source
var destinationFrames: [VTFrameProcessorFrame] { get }
```

## Discussion

This array must contain the same number of elements as the `interpolationPhase` property.

## See Also

### Inspecting the parameters

var sourceFrame: VTFrameProcessorFrame

The current source frame.

var nextFrame: VTFrameProcessorFrame?

The next source frame in presentation time order.

var opticalFlow: VTFrameProcessorOpticalFlow?

A property that defines the optical flow for an object.

var interpolationPhase: [Float]

An array of floating-point values that indicate which intervals to insert a frame between the current and next frame.

var submissionMode: VTFrameRateConversionParameters.SubmissionMode

A value describing the processing request in a parameters submission object.

enum SubmissionMode

A value describing the processing request in a parameters submission object.

