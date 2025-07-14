

- AVFoundation
- AVPartialAsyncProperty
-  minimumTimeOffsetFromLive 

Type Property

# minimumTimeOffsetFromLive

A time value that indicates how closely playback follows the latest live stream content.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var minimumTimeOffsetFromLive: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAsset`.

## Discussion

Use the load(_:) method to retrieve the property value.

This property value is only valid when working with live streaming content. For non-live assets, this property value is invalid.

## See Also

### Loading Duration and Timing

static var duration: AVAsyncProperty&lt;Root, CMTime>

A time value that represents the duration of the asset.

static var providesPreciseDurationAndTiming: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether the asset provides precise duration and timing.

