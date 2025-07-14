

- Vision
- VNVideoProcessor
-  addRequest(\_:processingOptions:) 

Instance Method

# addRequest(\_:processingOptions:)

Adds a request with processing options to the video processor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func addRequest(
    _ request: VNRequest,
    processingOptions: VNVideoProcessor.RequestProcessingOptions
) throws
```

## Parameters 

`request`  

The Vision request to add.

`processingOptions`  

The processing options to apply.

## Discussion

Call this method either before calling analyze(_:) or from within the completion handler of an already associated request.

## See Also

### Performing Requests

class RequestProcessingOptions

An object that defines a video processor’s configuration options.

func removeRequest(VNRequest) throws

Removes a Vision request from the video processor’s request queue.

func analyze(CMTimeRange) throws

Analyzes a time range of video content.

func cancel()

Cancels the video processing.

func add(VNRequest, withProcessingOptions: [VNVideoProcessingOption : Any]) throws

Adds a Vision request to perform with the specified configuration.

Deprecated

func analyze(with: CMTimeRange) throws

Analyzes the specifed time range of the video content.

Deprecated

