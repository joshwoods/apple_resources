

- SceneKit
- SCNParticleBirthDirection
-  SCNParticleBirthDirection.surfaceNormal 

Case

# SCNParticleBirthDirection.surfaceNormal

The emitting direction for each particle is along the surface normal vector at the point where the particle is emitted.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
case surfaceNormal
```

## Discussion

The particle system creates new particles at points in space defined by the emitterShape geometry. When a new particle is emitted, the geometry’s surface normal vector at the point nearest the particle determines the particle’s initial direction. (Note that the birthLocation property defines where particles may be created relative to the emitterShape geometry.)

This value has no effect if the emitterShape property value is `nil`.

## See Also

### Constants

case constant

The emitting direction is the same for all particles.

case random

SceneKit randomizes the emitting direction for each particle.

