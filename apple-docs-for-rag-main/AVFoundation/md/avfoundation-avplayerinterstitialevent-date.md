

- AVFoundation
- AVPlayerInterstitialEvent
-  date 

Instance Property

# date

A date within the date range of the primary content that playback of interstitial content begins.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var date: Date? { get set }
```

## Discussion

This property value is `nil` if you initialized the event with a time instead of a date.

## See Also

### Inspecting timing

var time: CMTime

A time within the timeline of the primary content that playback of interstitial content begins.

var willPlayOnce: Bool

A Boolean value that indicates whether to schedule this event one time only and suppress subsequent replay.

var resumptionOffset: CMTime

A time offset at which playback of primary content resumes after interstitial content finishes.

var playoutLimit: CMTime

The time offset at which playback of the interstitial ends.

var alignsStartWithPrimarySegmentBoundary: Bool

A Boolean value that indicates whether the start time of interstitial playback should snap to a segment boundary of the primary asset.

var alignsResumptionWithPrimarySegmentBoundary: Bool

A Boolean value that indicates whether the resumption time of primary playback should snap to a segment boundary of the primary asset.

