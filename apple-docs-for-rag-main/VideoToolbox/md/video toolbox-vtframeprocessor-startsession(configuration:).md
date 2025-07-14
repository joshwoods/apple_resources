

- Video Toolbox
- VTFrameProcessor
-  startSession(configuration:) 

Instance Method

# startSession(configuration:)

Starts a new session and configures the processor pipeline.

macOS 15.4+

``` source
func startSession(configuration: any VTFrameProcessorConfiguration) throws
```

## Parameters 

`configuration`  

A configuration object for the video effect that will be applied in the subsequent processing calls.

## See Also

### Processing frames

func process(parameters: any VTFrameProcessorParameters, completionHandler: (any VTFrameProcessorParameters, (any Error)?) -> Void)

Asynchronously performs the video effect specified in the start session.

func process(with: any MTLCommandBuffer, parameters: any VTFrameProcessorParameters)

Asynchronously performs the video effect specified in the start session specifically for Metal.

func endSession()

Performs all necessary tasks to end the session.

