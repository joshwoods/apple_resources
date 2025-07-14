

- SceneKit
-  SCNParticleSortingMode 

Enumeration

# SCNParticleSortingMode

Options for the rendering order of particles, used by the sortingMode property.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
enum SCNParticleSortingMode
```

## Topics

### Constants

case none

Particles are not sorted; they may be rendered in any order.

case projectedDepth

Particles farther from the point of view (as measured using projected depth) are rendered before closer particles.

case distance

Particles farther from the point of view (as measured using distance from the camera in scene space) are rendered before closer particles.

case oldestFirst

Particles emitted earlier are rendered before particles emitted more recently.

case youngestFirst

Particles emitted more recently are rendered before particles emitted earlier.

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

enum SCNParticleOrientationMode

Options for restricting the orientation of particles, used by the orientationMode property.

var sortingMode: SCNParticleSortingMode

The mode defining the order in which SceneKit renders the system’s particles.

var isLightingEnabled: Bool

A Boolean value that determines whether SceneKit applies lighting to particle images when rendering.

var isBlackPassEnabled: Bool

A Boolean value that determines whether SceneKit renders particles in black before rendering the particle image.

