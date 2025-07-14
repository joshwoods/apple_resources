

- SceneKit
- SCNParticleSystem
-  birthDirection 

Instance Property

# birthDirection

The possible initial directions for newly spawned particles, relative to the emitter shape.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var birthDirection: SCNParticleBirthDirection { get set }
```

## Discussion

This property defines initial directions for new particles relative to the geometry specified in the emitterShape property. This property has no effect if the emitterShape property value is `nil`.

For example, if the emitter shape is an SCNSphere geometry and the birth location is SCNParticleBirthDirection.surfaceNormal, new particles radiate away from the center of the sphere. You can randomize the direction of newly spawned particles with the spreadingAngle property.

The default value is SCNParticleBirthDirection.constant, specifying that all particles use the same base emittingDirection value. For possible values, see SCNParticleBirthDirection.

## See Also

### Managing Particle Emission Locations

var emitterShape: SCNGeometry?

The shape of the region of space where the system spawns new particles.

var birthLocation: SCNParticleBirthLocation

The possible locations for newly spawned particles, relative to the emitter shape.

enum SCNParticleBirthLocation

Options for the initial location of each emitted particle, used by the birthLocation property.

enum SCNParticleBirthDirection

Options for the initial direction of each emitted particle, used by the birthDirection property.

var emittingDirection: SCNVector3

The initial direction for newly spawned particles. Animatable.

var spreadingAngle: CGFloat

The range, in degrees, of randomized initial particle directions. Animatable.

