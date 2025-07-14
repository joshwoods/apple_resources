

- SceneKit
- SCNParticleSystem
-  emittingDirection 

Instance Property

# emittingDirection

The initial direction for newly spawned particles. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var emittingDirection: SCNVector3 { get set }
```

## Discussion

If the the emitterShape property value is `nil` or the birthDirection property value is SCNParticleBirthDirection.constant, newly spawned particles emit in the direction specified by this property. You can randomize the direction of newly spawned particles with the spreadingAngle property.

The default value is the vector `{0.0, 0.0, 1.0}`, specifying that particles emit in the direction of the positive z-axis.

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

var spreadingAngle: CGFloat

The range, in degrees, of randomized initial particle directions. Animatable.

