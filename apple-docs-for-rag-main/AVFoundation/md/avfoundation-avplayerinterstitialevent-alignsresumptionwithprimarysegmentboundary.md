

- AVFoundation
- AVPlayerInterstitialEvent
-  alignsResumptionWithPrimarySegmentBoundary 

Instance Property

# alignsResumptionWithPrimarySegmentBoundary

A Boolean value that indicates whether the resumption time of primary playback should snap to a segment boundary of the primary asset.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var alignsResumptionWithPrimarySegmentBoundary: Bool { get set }
```

## Discussion

If the value is true, the system adjusts the resumption time of primary playback following an interstitial to the nearest segment boundary when the primary player is playing an HTTP Live Streaming asset.

## See Also

### Inspecting timing

var time: CMTime

A time within the timeline of the primary content that playback of interstitial content begins.

var date: Date?

A date within the date range of the primary content that playback of interstitial content begins.

var willPlayOnce: Bool

A Boolean value that indicates whether to schedule this event one time only and suppress subsequent replay.

var resumptionOffset: CMTime

A time offset at which playback of primary content resumes after interstitial content finishes.

var playoutLimit: CMTime

The time offset at which playback of the interstitial ends.

var alignsStartWithPrimarySegmentBoundary: Bool

A Boolean value that indicates whether the start time of interstitial playback should snap to a segment boundary of the primary asset.

