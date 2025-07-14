

- AVFoundation
- AVPlayerItemSegment
-  loadedTimeRanges 

Instance Property

# loadedTimeRanges

The time ranges for the segment that have media data is readily available.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@nonobjc
var loadedTimeRanges: [CMTimeRange] { get }
```

## Discussion

The loaded time ranges might be discontinuous.

## See Also

### Inspecting the segment

var timeMapping: CMTimeMapping

The time mapping for this segment.

var startDate: Date?

The date at which a segment starts.

var interstitialEvent: AVPlayerInterstitialEvent?

The associated interstitial event for this segment.

