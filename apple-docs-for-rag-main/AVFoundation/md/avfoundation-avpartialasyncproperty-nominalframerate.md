

- AVFoundation
- AVPartialAsyncProperty
-  nominalFrameRate 

Type Property

# nominalFrameRate

The frame rate of the track, in frames per second.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var nominalFrameRate: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAssetTrack`.

## Discussion

Use the load(_:) method to retrieve the property value.

The nominal frame rate indicates the number of frames per second for tracks that contain a full frame per media sample. For field-based (interlaced) video tracks, the value of this property indicates the field rate, not the frame rate.

## See Also

### Loading Frame-Based Characteristics

static var minFrameDuration: AVAsyncProperty&lt;Root, CMTime>

The minimum duration of the track’s frames.

static var requiresFrameReordering: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether samples in the track may have different presentation and decode timestamps.

