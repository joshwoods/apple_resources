

- SceneKit
-  SCNBlendMode 

Enumeration

# SCNBlendMode

Modes that describe how SceneKit blends source colors rendered using a material with destination colors already in a rendering target, used by the blendMode property.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum SCNBlendMode
```

## Topics

### Constants

case alpha

Blend by multiplying source and destination color values by their corresponding alpha values.

case add

Blend by adding the source color to the destination color.

case subtract

Blend by subtracting the source color from the destination color.

case multiply

Blend by multiplying the source color with the background color.

case screen

Blend by multiplying the inverse of the source color with the inverse of the destination color.

case replace

Blend by replacing the destination color with the source color, ignoring alpha.

### Enumeration Cases

case max

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

### Managing Opacity and Blending

var transparency: CGFloat

The uniform transparency of the material. Animatable.

var transparencyMode: SCNTransparencyMode

The mode SceneKit uses to calculate transparency for the material.

enum SCNTransparencyMode

The modes SceneKit uses to calculate the opacity of pixels rendered with a material, used by the transparencyMode property.

var blendMode: SCNBlendMode

The mode that determines how pixel colors rendered using this material blend with other pixel colors in the rendering target.

