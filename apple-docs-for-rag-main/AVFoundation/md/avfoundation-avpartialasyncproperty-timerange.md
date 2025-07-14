

- AVFoundation
- AVPartialAsyncProperty
-  timeRange 

Type Property

# timeRange

The time range of the track within the overall timeline of the asset.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var timeRange: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAssetTrack`.

## Discussion

Use the load(_:) method to retrieve the property value.

If the start of the time range is greater than zero, the track doesn’t initially have media data to present. This condition may occur when the media delays an audio track to align the start of audio with a specific video frame. You can test for this as the example below shows:

```
if track.timeRange.start > .zero {
    // Delayed start.
}
```

## See Also

### Loading Temporal Information

static var naturalTimeScale: AVAsyncProperty&lt;Root, CMTimeScale>

The natural time scale of the media that a track references.

static var estimatedDataRate: AVAsyncProperty&lt;Root, Float>

The estimated data rate, in bits per second, of the media that the track references.

