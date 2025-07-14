

- SceneKit
- SCNParticleSystem
-  orientationMode 

Instance Property

# orientationMode

The mode defining whether and how particles may rotate.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var orientationMode: SCNParticleOrientationMode { get set }
```

## Discussion

A particle’s angle (or orientation) is independent from its direction of motion. For example, a smoke effect may use a small image of a cloud for each particle, which stays at the same angle as the smoke rises, but a snow effect may use an image that flips and rotates as each snowflake falls.

For possible orientation modes, see SCNParticleOrientationMode. The default value is SCNParticleOrientationMode.billboardScreenAligned.

## See Also

### Managing Particle Rendering

var blendMode: SCNParticleBlendMode

The blending mode for compositing particle images into the rendered scene.

enum SCNParticleBlendMode

Options for combining source and destination pixel colors when compositing particles during rendering, used by the blendMode property.

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

