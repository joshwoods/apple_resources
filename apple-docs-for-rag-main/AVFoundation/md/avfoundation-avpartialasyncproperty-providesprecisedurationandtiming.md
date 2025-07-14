

- AVFoundation
- AVPartialAsyncProperty
-  providesPreciseDurationAndTiming 

Type Property

# providesPreciseDurationAndTiming

A Boolean value that indicates whether the asset provides precise duration and timing.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var providesPreciseDurationAndTiming: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAsset`.

## Discussion

Use the load(_:) method to retrieve the property value.

This property value is true if you initialized the asset with the AVURLAssetPreferPreciseDurationAndTimingKey initialization option, otherwise it’s false.

Note

If calculating precise duration and timing isn’t possible for the media resources that the URL references, the value of this property is false, even if you requested otherwise.

## See Also

### Loading Duration and Timing

static var duration: AVAsyncProperty&lt;Root, CMTime>

A time value that represents the duration of the asset.

static var minimumTimeOffsetFromLive: AVAsyncProperty&lt;Root, CMTime>

A time value that indicates how closely playback follows the latest live stream content.

