

- AVFoundation
- AVPlayerInterstitialEvent
-  contentMayVary 

Instance Property

# contentMayVary

A Boolean value that indicates whether an event’s content is dynamic and the server may respond with different interstitial assets for other participants in a coordinated playback session.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var contentMayVary: Bool { get set }
```

## Discussion

If the value is false, the primary asset participates in coordinated playback, this event does as well.

The default value is true.

## See Also

### Inspecting timeline occupancy

var timelineOccupancy: AVPlayerInterstitialEvent.TimelineOccupancy

An event’s occupancy on the integrated timeline.

enum TimelineOccupancy

Constants that specify how an event occupies time on an integrated timeline.

var supplementsPrimaryContent: Bool

A Boolean value that indicates whether an event supplements the primary content and should present with the primary item.

var plannedDuration: CMTime

The planned duration of the event.

