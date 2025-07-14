

- SceneKit
- SCNParticleSystem
-  isBlackPassEnabled 

Instance Property

# isBlackPassEnabled

A Boolean value that determines whether SceneKit renders particles in black before rendering the particle image.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var isBlackPassEnabled: Bool { get set }
```

## Discussion

Set this property to true to enhance visual contrast when using additive blending. The default value is false.

Important

Because a black pass requires rendering the entire particle system twice, enabling this option can severely affect rendering performance.

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

var sortingMode: SCNParticleSortingMode

The mode defining the order in which SceneKit renders the system’s particles.

enum SCNParticleSortingMode

Options for the rendering order of particles, used by the sortingMode property.

var isLightingEnabled: Bool

A Boolean value that determines whether SceneKit applies lighting to particle images when rendering.

