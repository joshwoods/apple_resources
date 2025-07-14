

- RealityKit
- SpatialTrackingSession
-  SpatialTrackingSession.Configuration 

Structure

# SpatialTrackingSession.Configuration

A type for configuring the spatial tracking session.

iOS 18.0+iPadOS 18.0+visionOS 2.0+

``` source
struct Configuration
```

## Mentioned in 

Implementing scene understanding and reconstruction in your RealityKit app

## Topics

### Structures

struct AnchorCapability

A type that defines various anchor tracking capabilities.

struct SceneUnderstandingCapability

Defines how system behaviors can use scene unerstanding data for.

### Initializers

init(tracking: Set&lt;SpatialTrackingSession.Configuration.AnchorCapability>)

Creates a configuration with a set of anchor capabilities.

init(tracking: Set&lt;SpatialTrackingSession.Configuration.AnchorCapability>, sceneUnderstanding: Set&lt;SpatialTrackingSession.Configuration.SceneUnderstandingCapability>, camera: SpatialTrackingSession.Configuration.Camera)

Creates a configuration with anchor capabilities, scene-understanding capabilities, and camera feeds.

### Instance Properties

var debugDescription: String

A human-readable description of the configuration.

### Instance Methods

func arConfiguration() -> ARConfiguration?

func supportedConfiguration() -> SpatialTrackingSession.Configuration

### Enumerations

enum Camera

Defines the camera feed the RealityView renders.

### Default Implementations

CustomStringConvertible Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible

## See Also

### Spatial tracking

class SpatialTrackingSession

An object that incorporates spatial tracking capabilities into your RealityKit apps.

struct AnchorCapability

A type that defines various anchor tracking capabilities.

struct SceneUnderstandingCapability

Defines how system behaviors can use scene unerstanding data for.

enum Camera

Defines the camera feed the RealityView renders.

struct UnavailableCapabilities

A type that contains the unavailable capabilities of the current spatial tracking session.

