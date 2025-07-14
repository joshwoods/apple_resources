

- SpriteKit
-  SKParticleRenderOrder 

Enumeration

# SKParticleRenderOrder

The order to use when the emitter’s particles are rendered.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum SKParticleRenderOrder
```

## Topics

### Constants

case oldestLast

The particles are rendered from newest to oldest. This is the default value.

case oldestFirst

The particles are rendered from oldest to newest.

case dontCare

The particles can be rendered in any order. SpriteKit may choose to reorder the particles to improve rendering performance.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Enumerations

enum SKActionTimingMode

The modes that an action can use to adjust the apparent timing of the action.

enum SKAttributeType

Options that specify an attribute’s data type.

enum SKBlendMode

The modes that describe how the source and destination pixel colors are used to calculate the new destination color.

enum SKInterpolationMode

The modes used to interpolate between keyframes in the sequence.

enum SKLabelHorizontalAlignmentMode

Options for aligning text horizontally.

enum SKLabelVerticalAlignmentMode

Options for aligning text vertically.

enum SKRepeatMode

The modes used to determine how the sequence repeats.

enum SKSceneScaleMode

The modes that determine how the scene’s area is mapped to the view that presents it.

enum SKTextureFilteringMode

Texture filtering modes to use when the texture is drawn in a size other than its native size.

struct SKTileAdjacencyMask

An enumeration defining how neighboring tiles are automatically placed next to each other.

enum SKTileDefinitionRotation

The allowed rotations for a given tile.

enum SKTileSetType

An enumeration defining how tiles are arranged.

enum SKTransitionDirection

For some transitions, the direction in which the transition is performed.

enum SKUniformType

An enumerated type to identify the type of a uniform object.

enum SKNodeFocusBehavior

Options for the focusable states of a SpriteKit node.

