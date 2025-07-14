

- SceneKit
- SCNParticleSystem
-  isLightingEnabled 

Instance Property

# isLightingEnabled

A Boolean value that determines whether SceneKit applies lighting to particle images when rendering.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var isLightingEnabled: Bool { get set }
```

## Discussion

If true, SceneKit uses the position, color, and other attributes of SCNLight objects in the scene to shade each rendered particle image. Use this option to enhance volumetric effects such as smoke and fog.

The default value is false.

Note

SceneKit uses only one SCNLight object to illuminate rendered particles. Use the categoryBitMask of the node containing the particle system to control which light applies to the particles.

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

var isBlackPassEnabled: Bool

A Boolean value that determines whether SceneKit renders particles in black before rendering the particle image.

