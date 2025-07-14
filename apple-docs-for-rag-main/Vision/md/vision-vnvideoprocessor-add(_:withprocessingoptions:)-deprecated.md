

- Vision
- VNVideoProcessor
-  add(\_:withProcessingOptions:) Deprecated

Instance Method

# add(\_:withProcessingOptions:)

Adds a Vision request to perform with the specified configuration.

iOS 14.0–14.0DeprecatediPadOS 14.0–14.0DeprecatedMac Catalyst 14.0–14.0DeprecatedmacOS 11.0–11.0DeprecatedtvOS 14.0–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func add(
    _ request: VNRequest,
    withProcessingOptions processingOptions: [VNVideoProcessingOption : Any] = [:]
) throws
```

Deprecated

Use addRequest(_:processingOptions:) instead.

## Parameters 

`request`  

The request to add to the processing queue.

`processingOptions`  

The options to use for processing.

## Topics

### Video Processing Options

struct VNVideoProcessingOption

Options to pass to the video processor when adding requests.

## See Also

### Performing Requests

func addRequest(VNRequest, processingOptions: VNVideoProcessor.RequestProcessingOptions) throws

Adds a request with processing options to the video processor.

class RequestProcessingOptions

An object that defines a video processor’s configuration options.

func removeRequest(VNRequest) throws

Removes a Vision request from the video processor’s request queue.

func analyze(CMTimeRange) throws

Analyzes a time range of video content.

func cancel()

Cancels the video processing.

func analyze(with: CMTimeRange) throws

Analyzes the specifed time range of the video content.

Deprecated

