

- ARKit
- RoomTrackingProvider
-  allAnchors 

Instance Property

# allAnchors

An array of the room anchors the room-tracking provider is tracking.

visionOS 2.0+

``` source
final var allAnchors: [RoomAnchor] { get }
```

## See Also

### Inspecting a room-tracking provider

var anchorUpdates: AnchorUpdateSequence&lt;RoomAnchor>

An asynchronous sequence of room anchor updates.

var currentRoomAnchor: RoomAnchor?

The room a person is in currently, if any.

var description: String

A textual representation of this room tracking provider.

var state: DataProviderState

The state of a room-tracking provider.

