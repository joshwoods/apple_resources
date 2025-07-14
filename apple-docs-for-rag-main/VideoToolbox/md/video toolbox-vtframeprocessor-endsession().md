

- Video Toolbox
- VTFrameProcessor
-  endSession() 

Instance Method

# endSession()

Performs all necessary tasks to end the session.

macOS 15.4+

``` source
func endSession()
```

## Discussion

After this call completes, no new frames can be processed unless startSession(configuration:) is called again.

## See Also

### Processing frames

func startSession(configuration: any VTFrameProcessorConfiguration) throws

Starts a new session and configures the processor pipeline.

func process(parameters: any VTFrameProcessorParameters, completionHandler: (any VTFrameProcessorParameters, (any Error)?) -> Void)

Asynchronously performs the video effect specified in the start session.

func process(with: any MTLCommandBuffer, parameters: any VTFrameProcessorParameters)

Asynchronously performs the video effect specified in the start session specifically for Metal.

