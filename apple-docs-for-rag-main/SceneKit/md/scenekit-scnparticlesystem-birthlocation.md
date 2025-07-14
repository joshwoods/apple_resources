

- SceneKit
- SCNParticleSystem
-  birthLocation 

Instance Property

# birthLocation

The possible locations for newly spawned particles, relative to the emitter shape.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var birthLocation: SCNParticleBirthLocation { get set }
```

## Discussion

This property defines locations for spawning new particles relative to the geometry specified in the emitterShape property. This property has no effect if the emitterShape property value is `nil`.

For example, if the emitter shape is an SCNBox geometry and the birth location is SCNParticleBirthLocation.vertex, new particles may randomly spawn at any of the eight corners of the box.

The default value is SCNParticleBirthLocation.surface, specifying that new particles spawn at random locations along the surface of the emitterShape geometry. For possible values, see SCNParticleBirthLocation.

## See Also

### Managing Particle Emission Locations

var emitterShape: SCNGeometry?

The shape of the region of space where the system spawns new particles.

enum SCNParticleBirthLocation

Options for the initial location of each emitted particle, used by the birthLocation property.

var birthDirection: SCNParticleBirthDirection

The possible initial directions for newly spawned particles, relative to the emitter shape.

enum SCNParticleBirthDirection

Options for the initial direction of each emitted particle, used by the birthDirection property.

var emittingDirection: SCNVector3

The initial direction for newly spawned particles. Animatable.

var spreadingAngle: CGFloat

The range, in degrees, of randomized initial particle directions. Animatable.

