

- SpriteKit
- SKTexture
-  usesMipmaps 

Instance Property

# usesMipmaps

A Boolean value that indicates whether the texture attempts to generate mipmaps.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var usesMipmaps: Bool { get set }
```

## Discussion

The default value is false. If you set this to true, Sprite Kit creates mipmaps for the texture when it prepares the texture for rendering. Mipmaps take up additional memory (usually one-third more) but can improve rendering quality and performance when the texture is reduced in size (such as when you reduce the scale of a sprite rendered using the texture).

You can only request mipmaps if both of the texture’s dimensions are a power of two.

## See Also

### Configuring a Texture’s Behavior for Scaling

var filteringMode: SKTextureFilteringMode

The filtering mode used when the size of a sprite drawn with the texture is not drawn at the texture’s native size.

enum SKTextureFilteringMode

Texture filtering modes to use when the texture is drawn in a size other than its native size.

