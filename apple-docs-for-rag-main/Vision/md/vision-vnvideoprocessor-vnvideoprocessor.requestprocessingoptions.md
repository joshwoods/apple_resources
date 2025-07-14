

- Vision
- VNVideoProcessor
-  VNVideoProcessor.RequestProcessingOptions 

Class

# VNVideoProcessor.RequestProcessingOptions

An object that defines a video processor’s configuration options.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class RequestProcessingOptions
```

## Topics

### Configuring Options

var cadence: VNVideoProcessor.Cadence?

The cadence the video processor maintains to process the request.

class Cadence

An object that defines the cadence at which to process video.

class FrameRateCadence

An object that defines a frame-based cadence for processing a video stream.

class TimeIntervalCadence

An object that defines a time-based cadence for processing a video stream.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Performing Requests

func addRequest(VNRequest, processingOptions: VNVideoProcessor.RequestProcessingOptions) throws

Adds a request with processing options to the video processor.

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

