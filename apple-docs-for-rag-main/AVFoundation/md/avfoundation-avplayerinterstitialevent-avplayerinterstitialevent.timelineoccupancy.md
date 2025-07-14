

- AVFoundation
- AVPlayerInterstitialEvent
-  AVPlayerInterstitialEvent.TimelineOccupancy 

Enumeration

# AVPlayerInterstitialEvent.TimelineOccupancy

Constants that specify how an event occupies time on an integrated timeline.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
enum TimelineOccupancy
```

## Topics

### Values

case singlePoint

The event occupies a single point on the integrated timeline.

case fill

The event fills the integrated timeline with the duration of this event.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting timeline occupancy

var timelineOccupancy: AVPlayerInterstitialEvent.TimelineOccupancy

An event’s occupancy on the integrated timeline.

var supplementsPrimaryContent: Bool

A Boolean value that indicates whether an event supplements the primary content and should present with the primary item.

var contentMayVary: Bool

A Boolean value that indicates whether an event’s content is dynamic and the server may respond with different interstitial assets for other participants in a coordinated playback session.

var plannedDuration: CMTime

The planned duration of the event.

