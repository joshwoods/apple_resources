

- SpriteKit
- SKTexture
-  filteringMode 

Instance Property

# filteringMode

The filtering mode used when the size of a sprite drawn with the texture is not drawn at the texture’s native size.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var filteringMode: SKTextureFilteringMode { get set }
```

## Discussion

The possible values for this property are listed in SKTextureFilteringMode. The default value is SKTextureFilteringMode.linear where each pixel is drawn by using a linear filter of multiple texels in the texture. The other option is SKTextureFilteringMode.nearest where each pixel is drawn using the nearest point in the texture.

The figure below shows the effect of different filtering modes. The rabbit texture (original on left) has been scaled up five times. Node 1 has been scaled using SKTextureFilteringMode.nearest and node 2 has been scaled with SKTextureFilteringMode.linear.

## See Also

### Configuring a Texture’s Behavior for Scaling

enum SKTextureFilteringMode

Texture filtering modes to use when the texture is drawn in a size other than its native size.

var usesMipmaps: Bool

A Boolean value that indicates whether the texture attempts to generate mipmaps.

