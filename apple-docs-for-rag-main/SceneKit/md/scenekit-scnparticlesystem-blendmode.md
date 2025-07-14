

- SceneKit
- SCNParticleSystem
-  blendMode 

Instance Property

# blendMode

The blending mode for compositing particle images into the rendered scene.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var blendMode: SCNParticleBlendMode { get set }
```

## Discussion

Together with the sortingMode property, blend modes affect the appearance of overlapping particle images when rendered.

For possible blend modes, see SCNParticleBlendMode. The default value is SCNParticleBlendMode.additive.

## See Also

### Managing Particle Rendering

enum SCNParticleBlendMode

Options for combining source and destination pixel colors when compositing particles during rendering, used by the blendMode property.

var orientationMode: SCNParticleOrientationMode

The mode defining whether and how particles may rotate.

enum SCNParticleOrientationMode

Options for restricting the orientation of particles, used by the orientationMode property.

var sortingMode: SCNParticleSortingMode

The mode defining the order in which SceneKit renders the system’s particles.

enum SCNParticleSortingMode

Options for the rendering order of particles, used by the sortingMode property.

var isLightingEnabled: Bool

A Boolean value that determines whether SceneKit applies lighting to particle images when rendering.

var isBlackPassEnabled: Bool

A Boolean value that determines whether SceneKit renders particles in black before rendering the particle image.

