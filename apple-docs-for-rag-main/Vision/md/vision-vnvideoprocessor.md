

- Vision
-  VNVideoProcessor 

Class

# VNVideoProcessor

An object that performs offline analysis of video content.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class VNVideoProcessor
```

## Topics

### Creating a Video Processor

init(url: URL)

Creates a video processor to perform Vision requests against the specified video asset.

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

func analyze(with: CMTimeRange) throws

Analyzes the specifed time range of the video content.

Deprecated

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Utilities

struct VNComputeStage

Types that represent the compute stage.

class VNGeometryUtils

Utility methods to determine the geometries of various Vision types.

