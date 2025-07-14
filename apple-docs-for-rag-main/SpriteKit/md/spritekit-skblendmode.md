

- SpriteKit
-  SKBlendMode 

Enumeration

# SKBlendMode

The modes that describe how the source and destination pixel colors are used to calculate the new destination color.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOSvisionOS 1.0+watchOS 2.0+

``` source
enum SKBlendMode
```

## Topics

### Constants

case alpha

The source and destination colors are blended by multiplying the source alpha value.

case add

The source and destination colors are added together.

case subtract

The source color is subtracted from the destination color.

case multiply

The source color is multiplied by the destination color.

case multiplyX2

The source color is multiplied by the destination color and then doubled.

case screen

The source color is added to the destination color times the inverted source color.

case replace

The source color replaces the destination color.

### Enumeration Cases

case multiplyAlpha

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

### Enumerations

enum SKActionTimingMode

The modes that an action can use to adjust the apparent timing of the action.

enum SKAttributeType

Options that specify an attribute’s data type.

enum SKInterpolationMode

The modes used to interpolate between keyframes in the sequence.

enum SKLabelHorizontalAlignmentMode

Options for aligning text horizontally.

enum SKLabelVerticalAlignmentMode

Options for aligning text vertically.

enum SKParticleRenderOrder

The order to use when the emitter’s particles are rendered.

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

