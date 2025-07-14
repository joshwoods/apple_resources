

- Video Toolbox
- VTOpticalFlowParameters
-  init(sourceFrame:nextFrame:submissionMode:destinationOpticalFlow:) 

Initializer

# init(sourceFrame:nextFrame:submissionMode:destinationOpticalFlow:)

macOS 15.4+

``` source
init?(
    sourceFrame: VTFrameProcessorFrame,
    nextFrame: VTFrameProcessorFrame,
    submissionMode: VTOpticalFlowParameters.SubmissionMode,
    destinationOpticalFlow: VTFrameProcessorOpticalFlow
)
```

## Parameters 

`sourceFrame`  

The current source frame. This must be a non-nil value.

`nextFrame`  

The next source frame in presentation time order. This value can be set to nil for the last frame.

`submissionMode`  

A value describing the processing request in a parameters submission object.

`destinationOpticalFlow`  

A user allocated mutable optical flow that will receive the results.

