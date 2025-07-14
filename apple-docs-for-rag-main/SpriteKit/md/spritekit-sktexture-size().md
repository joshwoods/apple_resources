

- SpriteKit
- SKTexture
-  size() 

Instance Method

# size()

Gets the size of the texture.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func size() -> CGSize
```

## Return Value

The dimensions of the texture, measured in points.

## Mentioned in 

Loading and Using Textures

## Discussion

If the texture was created using an image file and that image file hasn’t been loaded, calling this method forces the texture data to be loaded from the file.

## See Also

### Reading a Texture’s Size and Optional Source Location

func textureRect() -> CGRect

Gets a rectangle that defines the portion of the texture used to render its image.

