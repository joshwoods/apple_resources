

- RealityKit
- SpatialTrackingSession
- SpatialTrackingSession.Configuration
-  SpatialTrackingSession.Configuration.AnchorCapability 

Structure

# SpatialTrackingSession.Configuration.AnchorCapability

A type that defines various anchor tracking capabilities.

iOS 18.0+iPadOS 18.0+visionOS 2.0+

``` source
struct AnchorCapability
```

## Topics

### Operators

static func == (SpatialTrackingSession.Configuration.AnchorCapability, SpatialTrackingSession.Configuration.AnchorCapability) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var debugDescription: String

A human-readable description of the anchor capability.

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static let body: SpatialTrackingSession.Configuration.AnchorCapability

The anchor capability that enables body tracking.

static let camera: SpatialTrackingSession.Configuration.AnchorCapability

The anchor capability that enables camera anchoring.

static let face: SpatialTrackingSession.Configuration.AnchorCapability

The anchor capability that enables face tracking.

static let hand: SpatialTrackingSession.Configuration.AnchorCapability

The anchor capability that enables hand tracking.

static let image: SpatialTrackingSession.Configuration.AnchorCapability

The anchor capability that enables image tracking.

static let object: SpatialTrackingSession.Configuration.AnchorCapability

The anchor capability that enables object tracking.

static let plane: SpatialTrackingSession.Configuration.AnchorCapability

The anchor capability that enables plane detection.

static let world: SpatialTrackingSession.Configuration.AnchorCapability

The anchor capability that enables world tracking.

### Default Implementations

CustomStringConvertible Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Spatial tracking

class SpatialTrackingSession

An object that incorporates spatial tracking capabilities into your RealityKit apps.

struct Configuration

A type for configuring the spatial tracking session.

struct SceneUnderstandingCapability

Defines how system behaviors can use scene unerstanding data for.

enum Camera

Defines the camera feed the RealityView renders.

struct UnavailableCapabilities

A type that contains the unavailable capabilities of the current spatial tracking session.

