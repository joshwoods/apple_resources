

- RealityKit
- SpatialTrackingSession
- SpatialTrackingSession.Configuration
-  SpatialTrackingSession.Configuration.Camera 

Enumeration

# SpatialTrackingSession.Configuration.Camera

Defines the camera feed the RealityView renders.

iOS 18.0+iPadOS 18.0+

``` source
enum Camera
```

## Topics

### Operators

static func == (SpatialTrackingSession.Configuration.Camera, SpatialTrackingSession.Configuration.Camera) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case back

The camera on the back of the device.

case front

The camera on the front of the device.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

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

struct UnavailableCapabilities

A type that contains the unavailable capabilities of the current spatial tracking session.

