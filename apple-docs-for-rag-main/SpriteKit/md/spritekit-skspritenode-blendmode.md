

- SpriteKit
- SKSpriteNode
-  blendMode 

Instance Property

# blendMode

The blend mode used to draw the sprite into the parent’s framebuffer.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var blendMode: SKBlendMode { get set }
```

**watchOS**

``` source
var blendMode: SKBlendMode { get set }
```

## Mentioned in 

Blending a Sprite with Different Interpretations of Alpha

## Discussion

The default value is SKBlendMode.alpha.

## See Also

### Configuring Alpha Blendling

Blending a Sprite with Different Interpretations of Alpha

Reinterpret a sprite’s alpha property to react differently to the objects below it.

enum SKBlendMode

The modes that describe how the source and destination pixel colors are used to calculate the new destination color.

