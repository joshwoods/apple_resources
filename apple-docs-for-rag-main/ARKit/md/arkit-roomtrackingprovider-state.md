

- ARKit
- RoomTrackingProvider
-  state 

Instance Property

# state

The state of a room-tracking provider.

visionOS 2.0+

``` source
final var state: DataProviderState { get }
```

## See Also

### Inspecting a room-tracking provider

var allAnchors: [RoomAnchor]

An array of the room anchors the room-tracking provider is tracking.

var anchorUpdates: AnchorUpdateSequence&lt;RoomAnchor>

An asynchronous sequence of room anchor updates.

var currentRoomAnchor: RoomAnchor?

The room a person is in currently, if any.

var description: String

A textual representation of this room tracking provider.

