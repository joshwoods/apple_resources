

- ARKit
- RoomTrackingProvider
-  currentRoomAnchor 

Instance Property

# currentRoomAnchor

The room a person is in currently, if any.

visionOS 2.0+

``` source
final var currentRoomAnchor: RoomAnchor? { get }
```

## See Also

### Inspecting a room-tracking provider

var allAnchors: [RoomAnchor]

An array of the room anchors the room-tracking provider is tracking.

var anchorUpdates: AnchorUpdateSequence&lt;RoomAnchor>

An asynchronous sequence of room anchor updates.

var description: String

A textual representation of this room tracking provider.

var state: DataProviderState

The state of a room-tracking provider.

