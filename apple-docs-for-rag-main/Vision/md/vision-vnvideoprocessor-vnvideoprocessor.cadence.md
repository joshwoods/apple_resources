

- Vision
- VNVideoProcessor
-  VNVideoProcessor.Cadence 

Class

# VNVideoProcessor.Cadence

An object that defines the cadence at which to process video.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class Cadence
```

## Relationships

### Inherits From

- NSObject

### Inherited By

- VNVideoProcessor.FrameRateCadence
- VNVideoProcessor.TimeIntervalCadence

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Configuring Options

var cadence: VNVideoProcessor.Cadence?

The cadence the video processor maintains to process the request.

class FrameRateCadence

An object that defines a frame-based cadence for processing a video stream.

class TimeIntervalCadence

An object that defines a time-based cadence for processing a video stream.

