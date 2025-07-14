

- AVFoundation
- AVPartialAsyncProperty
-  requiresFrameReordering 

Type Property

# requiresFrameReordering

A Boolean value that indicates whether samples in the track may have different presentation and decode timestamps.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var requiresFrameReordering: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAssetTrack`.

## Discussion

Use the load(_:) method to retrieve the property value.

## See Also

### Loading Frame-Based Characteristics

static var nominalFrameRate: AVAsyncProperty&lt;Root, Float>

The frame rate of the track, in frames per second.

static var minFrameDuration: AVAsyncProperty&lt;Root, CMTime>

The minimum duration of the track’s frames.

