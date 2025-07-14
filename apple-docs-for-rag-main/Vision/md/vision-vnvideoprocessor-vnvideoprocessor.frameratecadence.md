

- Vision
- VNVideoProcessor
-  VNVideoProcessor.FrameRateCadence 

Class

# VNVideoProcessor.FrameRateCadence

An object that defines a frame-based cadence for processing a video stream.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class FrameRateCadence
```

## Topics

### Creating a Cadence

init(Int)

Creates a new frame-based cadence with a frame rate.

### Inspecting the Frame Rate

var frameRate: Int

The frame rate at which to process video.

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

class TimeIntervalCadence

An object that defines a time-based cadence for processing a video stream.

