

- AVFoundation
- AVPlayerInterstitialEvent
-  timelineOccupancy 

Instance Property

# timelineOccupancy

An event’s occupancy on the integrated timeline.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var timelineOccupancy: AVPlayerInterstitialEvent.TimelineOccupancy { get set }
```

## Discussion

The default value is AVPlayerInterstitialEvent.TimelineOccupancy.singlePoint.

## See Also

### Inspecting timeline occupancy

enum TimelineOccupancy

Constants that specify how an event occupies time on an integrated timeline.

var supplementsPrimaryContent: Bool

A Boolean value that indicates whether an event supplements the primary content and should present with the primary item.

var contentMayVary: Bool

A Boolean value that indicates whether an event’s content is dynamic and the server may respond with different interstitial assets for other participants in a coordinated playback session.

var plannedDuration: CMTime

The planned duration of the event.

