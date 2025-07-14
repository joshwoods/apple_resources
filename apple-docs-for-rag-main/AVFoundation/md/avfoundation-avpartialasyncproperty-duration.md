

- AVFoundation
- AVPartialAsyncProperty
-  duration 

Type Property

# duration

A time value that represents the duration of the asset.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var duration: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAsset`.

## Discussion

Use the load(_:) method to retrieve the property value.

If the value of providesPreciseDurationAndTiming is false, the asset returns a best-available estimate of the duration. You can specify your preferred degree of precision for timing-related properties when you create an AVURLAsset by passing a value for the AVURLAssetPreferPreciseDurationAndTimingKey initialization option.

## See Also

### Loading Duration and Timing

static var providesPreciseDurationAndTiming: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether the asset provides precise duration and timing.

static var minimumTimeOffsetFromLive: AVAsyncProperty&lt;Root, CMTime>

A time value that indicates how closely playback follows the latest live stream content.

