

- SpriteKit
- SKSpriteNode
-  color 

Instance Property

# color

The sprite’s color.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
var color: UIColor { get set }
```

**macOS**

``` source
@MainActor
var color: NSColor { get set }
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
var color: UIColor { get set }
```

## Mentioned in 

Tinting a Sprite

## Discussion

If the texture property is non-`nil`, the red, green, and blue values of the color property are blended with the texture before the texture is drawn and the alpha property is ignored. If the texture property is `nil`, the color (including the alpha component) is used to draw a single-color rectangle.

## See Also

### Tinting a Sprite

Tinting a Sprite

Provide a color and blend factor to additively color your sprite.

var colorBlendFactor: CGFloat

A floating-point value that describes how the color is blended with the sprite’s texture.

