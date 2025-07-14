

- RealityKit
- SpatialTrackingSession
-  SpatialTrackingSession.UnavailableCapabilities 

Structure

# SpatialTrackingSession.UnavailableCapabilities

A type that contains the unavailable capabilities of the current spatial tracking session.

iOS 18.0+iPadOS 18.0+visionOS 2.0+

``` source
struct UnavailableCapabilities
```

## Topics

### Initializers

init()

Creates an unavailable capabilities instance.

### Instance Properties

var anchor: Set&lt;SpatialTrackingSession.Configuration.AnchorCapability>

A type that contains all unavailable anchor capabilities.

var debugDescription: String

var missingAuthorizations: Set&lt;ARKitSession.AuthorizationType>

The set of requested ARKit authorizations that the user doesn’t approve.

var missingCameraAuthorization: Bool?

Whether the person using the device approves the camera authorization or not.

var sceneUnderstanding: Set&lt;SpatialTrackingSession.Configuration.SceneUnderstandingCapability>

A type that contains all unavailable scene-understanding capabilities.

### Default Implementations

CustomStringConvertible Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Sendable

## See Also

### Spatial tracking

class SpatialTrackingSession

An object that incorporates spatial tracking capabilities into your RealityKit apps.

struct Configuration

A type for configuring the spatial tracking session.

struct AnchorCapability

A type that defines various anchor tracking capabilities.

struct SceneUnderstandingCapability

Defines how system behaviors can use scene unerstanding data for.

enum Camera

Defines the camera feed the RealityView renders.

