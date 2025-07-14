

- ARKit
- RoomTrackingProvider
-  description 

Instance Property

# description

A textual representation of this room tracking provider.

visionOS 2.0+

``` source
final var description: String { get }
```

## See Also

### Inspecting a room-tracking provider

var allAnchors: [RoomAnchor]

An array of the room anchors the room-tracking provider is tracking.

var anchorUpdates: AnchorUpdateSequence&lt;RoomAnchor>

An asynchronous sequence of room anchor updates.

var currentRoomAnchor: RoomAnchor?

The room a person is in currently, if any.

var state: DataProviderState

The state of a room-tracking provider.

