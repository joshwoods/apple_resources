

- Vision
- VNVideoProcessor
-  analyze(\_:) 

Instance Method

# analyze(\_:)

Analyzes a time range of video content.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func analyze(_ timeRange: CMTimeRange) throws
```

## Parameters 

`timeRange`  

The time range to analyze. The value must be within the time range of the video asset.

## Discussion

The system executes this method synchronously, so you typically call it from a separate dispatch queue. It returns when the video processor finishes analyzing the time range or if an error prevents processing.

## See Also

### Performing Requests

func addRequest(VNRequest, processingOptions: VNVideoProcessor.RequestProcessingOptions) throws

Adds a request with processing options to the video processor.

class RequestProcessingOptions

An object that defines a video processor’s configuration options.

func removeRequest(VNRequest) throws

Removes a Vision request from the video processor’s request queue.

func cancel()

Cancels the video processing.

func add(VNRequest, withProcessingOptions: [VNVideoProcessingOption : Any]) throws

Adds a Vision request to perform with the specified configuration.

Deprecated

func analyze(with: CMTimeRange) throws

Analyzes the specifed time range of the video content.

Deprecated

