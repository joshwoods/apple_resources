

- Vision
- VNVideoProcessor
-  removeRequest(\_:) 

Instance Method

# removeRequest(\_:)

Removes a Vision request from the video processor’s request queue.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func removeRequest(_ request: VNRequest) throws
```

## Parameters 

`request`  

The request to remove.

## See Also

### Performing Requests

func addRequest(VNRequest, processingOptions: VNVideoProcessor.RequestProcessingOptions) throws

Adds a request with processing options to the video processor.

class RequestProcessingOptions

An object that defines a video processor’s configuration options.

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

