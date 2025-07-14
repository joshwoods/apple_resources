

- AVFoundation
- AVPlayerItemSegment
-  interstitialEvent 

Instance Property

# interstitialEvent

The associated interstitial event for this segment.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var interstitialEvent: AVPlayerInterstitialEvent? { get }
```

## Discussion

This value is `nil` for segments that represent playback of the primary item.

## See Also

### Inspecting the segment

var timeMapping: CMTimeMapping

The time mapping for this segment.

var loadedTimeRanges: [CMTimeRange]

The time ranges for the segment that have media data is readily available.

var startDate: Date?

The date at which a segment starts.

