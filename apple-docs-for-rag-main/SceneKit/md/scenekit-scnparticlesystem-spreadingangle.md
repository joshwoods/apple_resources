

- SceneKit
- SCNParticleSystem
-  spreadingAngle 

Instance Property

# spreadingAngle

The range, in degrees, of randomized initial particle directions. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var spreadingAngle: CGFloat { get set }
```

## Discussion

Setting a nonzero value for this property randomizes the direction specified by the emittingDirection or birthDirection property. For example, at the default value of `0.0` degrees, all particles emit in the same direction. Increasing the spreading angle to `30.0` degrees allows particles to emit in any direction within a space shaped like a cone whose central angle is 30°.

This property has no effect if the birthDirection property value is SCNParticleBirthDirection.random.

You can animate changes to this property’s value. See Animating SceneKit Content.

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

enum SCNParticleBirthDirection

Options for the initial direction of each emitted particle, used by the birthDirection property.

var emittingDirection: SCNVector3

The initial direction for newly spawned particles. Animatable.

