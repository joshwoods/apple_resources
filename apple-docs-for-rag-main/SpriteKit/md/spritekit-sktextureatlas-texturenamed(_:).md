

- SpriteKit
- SKTextureAtlas
-  textureNamed(\_:) 

Instance Method

# textureNamed(\_:)

Creates a texture from data stored in the texture atlas.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func textureNamed(_ name: String) -> SKTexture
```

## Parameters 

`name`  

The name of a texture stored in the atlas object.

## Return Value

The SpriteKit texture associated with the name. If the specified image does not exist in the atlas object, SpriteKit returns a placeholder texture image.

## Mentioned in 

Maximizing Node Drawing Performance

About Texture Atlases

