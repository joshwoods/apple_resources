

- SceneKit
- SCNParticleBirthDirection
-  SCNParticleBirthDirection.constant 

Case

# SCNParticleBirthDirection.constant

The emitting direction is the same for all particles.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
case constant
```

## Discussion

When using this mode, the emittingDirection property determines the base direction for all particles, and the spreadingAngle property adds random variation to this direction.

## See Also

### Constants

case surfaceNormal

The emitting direction for each particle is along the surface normal vector at the point where the particle is emitted.

case random

SceneKit randomizes the emitting direction for each particle.

