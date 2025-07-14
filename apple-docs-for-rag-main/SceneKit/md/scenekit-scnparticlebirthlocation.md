

- SceneKit
-  SCNParticleBirthLocation 

Enumeration

# SCNParticleBirthLocation

Options for the initial location of each emitted particle, used by the birthLocation property.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
enum SCNParticleBirthLocation
```

## Overview

The emitterShape property determines the shape of the space in which new particles can be emitted, and the birthLocation property determines the locations of new particles relative to this shape.

To make a system’s particles emit from a single point, set the emitterShape property to `nil` (the default). In this case, SceneKit ignores the birthLocation property.

## Topics

### Constants

case surface

New particles can be created at any location on the surface of the emitter shape.

case volume

New particles can be created at any location within the volume of the emitter shape.

case vertex

New particles can be created at only at the locations of the vertices in the emitter shape.

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

var birthDirection: SCNParticleBirthDirection

The possible initial directions for newly spawned particles, relative to the emitter shape.

enum SCNParticleBirthDirection

Options for the initial direction of each emitted particle, used by the birthDirection property.

var emittingDirection: SCNVector3

The initial direction for newly spawned particles. Animatable.

var spreadingAngle: CGFloat

The range, in degrees, of randomized initial particle directions. Animatable.

