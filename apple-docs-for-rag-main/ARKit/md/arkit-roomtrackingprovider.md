

- ARKit
-  RoomTrackingProvider 

Class

# RoomTrackingProvider

A source of real-time information about the room that a person is currently in.

visionOS 2.0+

``` source
final class RoomTrackingProvider
```

## Topics

### Creating a room-tracking provider

init()

Creates a room-tracking provider.

### Inspecting a room-tracking provider

var allAnchors: [RoomAnchor]

An array of the room anchors the room-tracking provider is tracking.

var anchorUpdates: AnchorUpdateSequence&lt;RoomAnchor>

An asynchronous sequence of room anchor updates.

var currentRoomAnchor: RoomAnchor?

The room a person is in currently, if any.

var description: String

A textual representation of this room tracking provider.

var state: DataProviderState

The state of a room-tracking provider.

### Type properties

static var isSupported: Bool

A Boolean values that indicates whether a device supports the room-tracking provider.

static var requiredAuthorizations: [ARKitSession.AuthorizationType]

An array of authorization types the room-tracking provider requires.

## Relationships

### Conforms To

- CustomStringConvertible
- DataProvider
- Sendable

## See Also

### Room tracking

struct RoomAnchor

The representation of a room ARKit is currently tracking.

Building local experiences with room tracking

Use room tracking in visionOS to provide custom interactions with physical spaces.

