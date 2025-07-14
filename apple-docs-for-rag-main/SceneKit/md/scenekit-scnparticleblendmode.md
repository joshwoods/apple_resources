

- SceneKit
-  SCNParticleBlendMode 

Enumeration

# SCNParticleBlendMode

Options for combining source and destination pixel colors when compositing particles during rendering, used by the blendMode property.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
enum SCNParticleBlendMode
```

## Topics

### Constants

case additive

The source and destination colors are added together.

case subtract

The source color is subtracted from the destination color.

case multiply

The source color is multiplied by the destination color.

case screen

The source color is added to the destination color times the inverted source color.

case alpha

The source and destination colors are blended by multiplying the source alpha value.

case replace

The source color replaces the destination color.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing Particle Rendering

var blendMode: SCNParticleBlendMode

The blending mode for compositing particle images into the rendered scene.

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

