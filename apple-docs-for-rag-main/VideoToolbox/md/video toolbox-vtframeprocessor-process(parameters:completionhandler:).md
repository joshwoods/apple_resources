

- Video Toolbox
- VTFrameProcessor
-  process(parameters:completionHandler:) 

Instance Method

# process(parameters:completionHandler:)

Asynchronously performs the video effect specified in the start session.

macOS 15.4+

``` source
func process(
    parameters: any VTFrameProcessorParameters,
    completionHandler: @escaping (any VTFrameProcessorParameters, (any Error)?) -> Void
)
```

``` source
func process(parameters: any VTFrameProcessorParameters) async throws -> any VTFrameProcessorParameters
```

## Parameters 

`parameters`  

A VTFrameProcessorParameters object to specify additional parameters to use during processing. It needs to match the configuration type used during start session.

`completionHandler`  

This completion handler is called when the frame processing is completed. The completion handler will receive the same parameters object that was provided to the original call, as well as an NSError which will contain an error code if processing was not successful.

## See Also

### Processing frames

func startSession(configuration: any VTFrameProcessorConfiguration) throws

Starts a new session and configures the processor pipeline.

func process(with: any MTLCommandBuffer, parameters: any VTFrameProcessorParameters)

Asynchronously performs the video effect specified in the start session specifically for Metal.

func endSession()

Performs all necessary tasks to end the session.

