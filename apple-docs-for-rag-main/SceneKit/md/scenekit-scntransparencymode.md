

- SceneKit
-  SCNTransparencyMode 

Enumeration

# SCNTransparencyMode

The modes SceneKit uses to calculate the opacity of pixels rendered with a material, used by the transparencyMode property.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum SCNTransparencyMode
```

## Topics

### Constants

case aOne

SceneKit derives transparency information from the alpha channel of colors. The value `1.0` is opaque.

case rgbZero

SceneKit derives transparency information from the luminance of colors. The value `0.0` is opaque.

### Enumeration Cases

case dualLayer

case singleLayer

### Initializers

init?(rawValue: Int)

### Type Properties

static var `default`: SCNTransparencyMode

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

var blendMode: SCNBlendMode

The mode that determines how pixel colors rendered using this material blend with other pixel colors in the rendering target.

enum SCNBlendMode

Modes that describe how SceneKit blends source colors rendered using a material with destination colors already in a rendering target, used by the blendMode property.

