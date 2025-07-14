

- SpriteKit
- SKTexture
-  textureRect() 

Instance Method

# textureRect()

Gets a rectangle that defines the portion of the texture used to render its image.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func textureRect() -> CGRect
```

## Return Value

A rectangle in the unit coordinate space.

## Discussion

The default value is a rectangle that covers the entire texture `(0,0)` - `(1,1)`. You cannot set this value directly; to use only a portion of a texture, use the init(rect:in:) method to create a new texture.

## See Also

### Reading a Texture’s Size and Optional Source Location

func size() -> CGSize

Gets the size of the texture.

