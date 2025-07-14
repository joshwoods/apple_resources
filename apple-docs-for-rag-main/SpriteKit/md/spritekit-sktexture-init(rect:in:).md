

- SpriteKit
- SKTexture
-  init(rect:in:) 

Initializer

# init(rect:in:)

Creates a new texture from a sub-rectangle of an existing texture.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
convenience init(
    rect: CGRect,
    in texture: SKTexture
)
```

## Parameters 

`rect`  

A rectangle in the unit coordinate space that specifies the portion of the texture to use.

`texture`  

The texture to create the new texture from.

## Return Value

A new texture object.

## Mentioned in 

Maximizing Node Drawing Performance

## Discussion

The returned texture object shares the same texture data as the original texture object, meaning that only one copy of the texture data is kept in memory.

If you call this method on a texture that itself was created using this method, the original texture is used as the source instead. That is, the rectangle is considered to be in the source texture’s coordinate system. To do this, you should use the source texture’s textureRect() rather than relying on hard coded `{(0,0) (1,1)}` as the coordinates.

Listing 1 shows, in Swift, how you can use the source texture’s textureRect() to calculate the portion of the texture to use.

Listing 1. Creating a texture from a portion of another texture.

```
let originalTexture = SKTexture(imageNamed: "sourceImage.png")

let rect = CGRect(origin: originalTexture.textureRect().origin,
                  size: CGSize(width: originalTexture.textureRect().midX,
                               height: originalTexture.textureRect().midY))

let croppedTexture = SKTexture(rect: rect,
                               in: originalTexture)
```

In the above example, if `originalTexture` had a size of `(348.0, 282.0)` and a textureRect() of `{(0,0) (1,1)}`, `croppedTexture` will have a size of `(174.0, 141.0)` and a textureRect() of `{(0,0) (1,1)}`. `croppedTexture` will be a copy of the bottom left quadrant of `originalTexture`.

