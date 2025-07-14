

- AVFoundation
- AVPartialAsyncProperty
-  minFrameDuration 

Type Property

# minFrameDuration

The minimum duration of the track’s frames.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var minFrameDuration: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAssetTrack`.

## Discussion

Use the load(_:) method to retrieve the property value.

A track’s minimum frame duration is the reciprocal of its maximum frame rate. For example, a video track with a maximum frame rate of 30 frames per second has a minimum frame duration of 1/30, or 0.033 seconds.

The value of this property is invalid if the track can’t calculate its minimum frame duration, or if it’s unknown.

## See Also

### Loading Frame-Based Characteristics

static var nominalFrameRate: AVAsyncProperty&lt;Root, Float>

The frame rate of the track, in frames per second.

static var requiresFrameReordering: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether samples in the track may have different presentation and decode timestamps.

