

- SceneKit
- SCNParticleSystem
-  emitterShape 

Instance Property

# emitterShape

The shape of the region of space where the system spawns new particles.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var emitterShape: SCNGeometry? { get set }
```

## Discussion

To randomize the locations where new particles spawn, assign a geometry to this property. This geometry defines the shape of the space where new particles may spawn, and the birthLocation and birthDirection properties define locations within and directions relative to the shape. For example, assigning a sphere geometry causes particles to spawn at random locations along the surface of the sphere (or within the volume of the sphere, according to the birthLocation property).

Note

For best results, use an instance of one of the SceneKit basic geometry classes (SCNPlane, SCNBox, SCNSphere, SCNPyramid, SCNCone, SCNCylinder, SCNCapsule, SCNTube, and SCNTorus). These classes provide a more efficient simulation and more even appearance to the rendered particle system.

The default value is `nil`, specifying that all new particles emit from a single point. For particle systems attached to a node, this point is the origin of the node’s coordinate system. For particle systems attached directly to a scene using the addParticleSystem(_:transform:) method, use that method’s `transform` parameter to specify the emission point.

## See Also

### Managing Particle Emission Locations

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

var spreadingAngle: CGFloat

The range, in degrees, of randomized initial particle directions. Animatable.

