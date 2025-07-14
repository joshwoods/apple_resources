

- Vision
- VNVideoProcessor
- VNVideoProcessor.RequestProcessingOptions
-  cadence 

Instance Property

# cadence

The cadence the video processor maintains to process the request.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
@NSCopying
var cadence: VNVideoProcessor.Cadence? { get set }
```

## Discussion

By default, the system processes every frame of video if you don’t provide a value for this property.

## See Also

### Configuring Options

class Cadence

An object that defines the cadence at which to process video.

class FrameRateCadence

An object that defines a frame-based cadence for processing a video stream.

class TimeIntervalCadence

An object that defines a time-based cadence for processing a video stream.

