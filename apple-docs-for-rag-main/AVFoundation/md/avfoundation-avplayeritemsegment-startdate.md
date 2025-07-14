

- AVFoundation
- AVPlayerItemSegment
-  startDate 

Instance Property

# startDate

The date at which a segment starts.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var startDate: Date? { get }
```

## Discussion

This value is `nil` if the primary item doesn’t contain dates.

## See Also

### Inspecting the segment

var timeMapping: CMTimeMapping

The time mapping for this segment.

var loadedTimeRanges: [CMTimeRange]

The time ranges for the segment that have media data is readily available.

var interstitialEvent: AVPlayerInterstitialEvent?

The associated interstitial event for this segment.

