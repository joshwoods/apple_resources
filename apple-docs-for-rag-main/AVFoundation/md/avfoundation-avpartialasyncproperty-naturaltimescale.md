

- AVFoundation
- AVPartialAsyncProperty
-  naturalTimeScale 

Type Property

# naturalTimeScale

The natural time scale of the media that a track references.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var naturalTimeScale: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAssetTrack`.

## Discussion

Use the load(_:) method to retrieve the property value.

## See Also

### Loading Temporal Information

static var timeRange: AVAsyncProperty&lt;Root, CMTimeRange>

The time range of the track within the overall timeline of the asset.

static var estimatedDataRate: AVAsyncProperty&lt;Root, Float>

The estimated data rate, in bits per second, of the media that the track references.

