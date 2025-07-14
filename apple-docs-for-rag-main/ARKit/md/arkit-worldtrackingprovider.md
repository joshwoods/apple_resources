

- ARKit
-  WorldTrackingProvider 

Class

# WorldTrackingProvider

A source of live data about the device pose and anchors in a person’s surroundings.

visionOS 1.0+

``` source
final class WorldTrackingProvider
```

## Topics

### Tracking objects

init()

Creates a world-tracking provider.

var anchorUpdates: AnchorUpdateSequence&lt;WorldAnchor>

A sequence of updates to anchors a provider tracks.

static var requiredAuthorizations: [ARKitSession.AuthorizationType]

The types of authorizations necessary for tracking world anchors.

static var isSupported: Bool

A Boolean value that indicates whether the current runtime environment supports world-tracking providers.

var allAnchors: [WorldAnchor]?

An array of all known world anchors from the world-tracking provider.

func addAnchor(WorldAnchor) async throws

Adds a world anchor you supply to the set of currently tracked anchors.

struct Error

An error that can occur during a world-tracking session.

### Stopping object tracking

func removeAnchor(WorldAnchor) async throws

Removes a world anchor from a world-tracking provider.

func removeAnchor(forID: UUID) async throws

Removes a world anchor from a world-tracking provider based on its ID.

### Predicting device pose

func queryDeviceAnchor(atTimestamp: TimeInterval) -> DeviceAnchor?

The predicted pose of the current device at a given time.

### Inspecting a world-tracking provider

var state: DataProviderState

The current status of data coming from a provider.

var description: String

A textual description of a world-tracking provider.

## Relationships

### Conforms To

- CustomStringConvertible
- DataProvider
- Sendable

## See Also

### World tracking

Tracking specific points in world space

Retrieve the position and orientation of anchors your app stores in ARKit.

struct WorldAnchor

A fixed location in a person’s surroundings.

struct DeviceAnchor

The position and orientation of Apple Vision Pro.

