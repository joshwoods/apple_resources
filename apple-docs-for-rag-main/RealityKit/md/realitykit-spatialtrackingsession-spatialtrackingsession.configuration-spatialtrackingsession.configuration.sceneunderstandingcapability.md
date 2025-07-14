

- RealityKit
- SpatialTrackingSession
- SpatialTrackingSession.Configuration
-  SpatialTrackingSession.Configuration.SceneUnderstandingCapability 

Structure

# SpatialTrackingSession.Configuration.SceneUnderstandingCapability

Defines how system behaviors can use scene unerstanding data for.

iOS 18.0+iPadOS 18.0+

``` source
struct SceneUnderstandingCapability
```

## Topics

### Operators

static func == (SpatialTrackingSession.Configuration.SceneUnderstandingCapability, SpatialTrackingSession.Configuration.SceneUnderstandingCapability) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var debugDescription: String

A human-readable description of the scene-understanding capability.

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static let collision: SpatialTrackingSession.Configuration.SceneUnderstandingCapability

The capability that allows the system to use scene-understanding data for collisions.

static let occlusion: SpatialTrackingSession.Configuration.SceneUnderstandingCapability

The capability that allows the system to use scene-understanding data for occlusion.

static let physics: SpatialTrackingSession.Configuration.SceneUnderstandingCapability

The capability that allows the system to use scene-understanding data for physics simulation.

static let shadow: SpatialTrackingSession.Configuration.SceneUnderstandingCapability

The capability that allows the system to use scene-understanding data for shadow casting.

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

struct AnchorCapability

A type that defines various anchor tracking capabilities.

enum Camera

Defines the camera feed the RealityView renders.

struct UnavailableCapabilities

A type that contains the unavailable capabilities of the current spatial tracking session.

