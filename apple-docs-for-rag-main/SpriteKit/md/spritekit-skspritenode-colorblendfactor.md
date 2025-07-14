

- SpriteKit
- SKSpriteNode
-  colorBlendFactor 

Instance Property

# colorBlendFactor

A floating-point value that describes how the color is blended with the sprite’s texture.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var colorBlendFactor: CGFloat { get set }
```

**watchOS**

``` source
var colorBlendFactor: CGFloat { get set }
```

## Mentioned in 

Tinting a Sprite

## Discussion

The value must be a number between `0.0` and `1.0`, inclusive. The default value (`0.0`) indicates the color property is ignored and that the texture’s values should be used unmodified. For values greater than `0.0`, the texture is blended with the color before being drawn to the scene.

## See Also

### Tinting a Sprite

Tinting a Sprite

Provide a color and blend factor to additively color your sprite.

var color: UIColor

The sprite’s color.

