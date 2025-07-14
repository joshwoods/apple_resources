

- SceneKit
-  SCNParticleOrientationMode 

Enumeration

# SCNParticleOrientationMode

Options for restricting the orientation of particles, used by the orientationMode property.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
enum SCNParticleOrientationMode
```

## Topics

### Constants

case billboardScreenAligned

Each particle’s orientation is always fixed with respect to the point of view camera.

case billboardViewAligned

Each particle always faces the point of view camera (but may rotate about an axis parallel to the view direction).

case free

Particle orientations are not restricted; they may rotate freely in all axes.

case billboardYAligned

The y-axis direction of each particle is always fixed with respect to the point of view camera.

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

enum SCNParticleBlendMode

Options for combining source and destination pixel colors when compositing particles during rendering, used by the blendMode property.

var orientationMode: SCNParticleOrientationMode

The mode defining whether and how particles may rotate.

var sortingMode: SCNParticleSortingMode

The mode defining the order in which SceneKit renders the system’s particles.

enum SCNParticleSortingMode

Options for the rendering order of particles, used by the sortingMode property.

var isLightingEnabled: Bool

A Boolean value that determines whether SceneKit applies lighting to particle images when rendering.

var isBlackPassEnabled: Bool

A Boolean value that determines whether SceneKit renders particles in black before rendering the particle image.

