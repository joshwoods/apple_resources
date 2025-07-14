

- Vision
- VNVideoProcessor
-  analyze(with:) Deprecated

Instance Method

# analyze(with:)

Analyzes the specifed time range of the video content.

iOS 14.0–14.0DeprecatediPadOS 14.0–14.0DeprecatedMac Catalyst 14.0–14.0DeprecatedmacOS 11.0–11.0DeprecatedtvOS 14.0–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func analyze(with timeRange: CMTimeRange) throws
```

Deprecated

Use analyze(_:) instead.

## Parameters 

`timeRange`  

The time range to analyze. The value specified must be within the time range of the video asset.

## Discussion

The system executes this method synchronously, so you should typically call it from a separate dispatch queue. It returns when the video processor finishes analyzing the specified time range, or if an error prevented the processing.

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

func add(VNRequest, withProcessingOptions: [VNVideoProcessingOption : Any]) throws

Adds a Vision request to perform with the specified configuration.

Deprecated

