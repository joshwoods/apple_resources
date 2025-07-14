

- SceneKit
- SCNParticleSystem
-  sortingMode 

Instance Property

# sortingMode

The mode defining the order in which SceneKit renders the system’s particles.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var sortingMode: SCNParticleSortingMode { get set }
```

## Discussion

Together with the blendMode property, sorting modes affect the appearance of overlapping particle images when rendered.

For possible sorting modes, see SCNParticleSortingMode. The default value is SCNParticleSortingMode.none, specifying that SceneKit may render particles in arbitrary order.

## See Also

### Managing Particle Rendering

var blendMode: SCNParticleBlendMode

The blending mode for compositing particle images into the rendered scene.

enum SCNParticleBlendMode

Options for combining source and destination pixel colors when compositing particles during rendering, used by the blendMode property.

var orientationMode: SCNParticleOrientationMode

The mode defining whether and how particles may rotate.

enum SCNParticleOrientationMode

Options for restricting the orientation of particles, used by the orientationMode property.

enum SCNParticleSortingMode

Options for the rendering order of particles, used by the sortingMode property.

var isLightingEnabled: Bool

A Boolean value that determines whether SceneKit applies lighting to particle images when rendering.

var isBlackPassEnabled: Bool

A Boolean value that determines whether SceneKit renders particles in black before rendering the particle image.

