

- Vision
- VNVideoProcessor
-  VNVideoProcessor.TimeIntervalCadence 

Class

# VNVideoProcessor.TimeIntervalCadence

An object that defines a time-based cadence for processing a video stream.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class TimeIntervalCadence
```

## Topics

### Creating a Cadence

init(CFTimeInterval)

Creates a new time-based cadence with a time interval.

### Inspecting the Time Interval

var timeInterval: CFTimeInterval

The time interval of the cadence.

## Relationships

### Inherits From

- VNVideoProcessor.Cadence

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

class Cadence

An object that defines the cadence at which to process video.

class FrameRateCadence

An object that defines a frame-based cadence for processing a video stream.

