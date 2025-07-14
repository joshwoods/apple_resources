

- SceneKit
-  SCNParticleBirthDirection 

Enumeration

# SCNParticleBirthDirection

Options for the initial direction of each emitted particle, used by the birthDirection property.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
enum SCNParticleBirthDirection
```

## Topics

### Constants

case constant

The emitting direction is the same for all particles.

case surfaceNormal

The emitting direction for each particle is along the surface normal vector at the point where the particle is emitted.

case random

SceneKit randomizes the emitting direction for each particle.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing Particle Emission Locations

var emitterShape: SCNGeometry?

The shape of the region of space where the system spawns new particles.

var birthLocation: SCNParticleBirthLocation

The possible locations for newly spawned particles, relative to the emitter shape.

enum SCNParticleBirthLocation

Options for the initial location of each emitted particle, used by the birthLocation property.

var birthDirection: SCNParticleBirthDirection

The possible initial directions for newly spawned particles, relative to the emitter shape.

var emittingDirection: SCNVector3

The initial direction for newly spawned particles. Animatable.

var spreadingAngle: CGFloat

The range, in degrees, of randomized initial particle directions. Animatable.

