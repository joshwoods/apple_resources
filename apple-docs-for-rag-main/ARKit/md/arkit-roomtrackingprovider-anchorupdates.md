

- ARKit
- RoomTrackingProvider
-  anchorUpdates 

Instance Property

# anchorUpdates

An asynchronous sequence of room anchor updates.

visionOS 2.0+

``` source
final var anchorUpdates: AnchorUpdateSequence { get }
```

## See Also

### Inspecting a room-tracking provider

var allAnchors: [RoomAnchor]

An array of the room anchors the room-tracking provider is tracking.

var currentRoomAnchor: RoomAnchor?

The room a person is in currently, if any.

var description: String

A textual representation of this room tracking provider.

var state: DataProviderState

The state of a room-tracking provider.

