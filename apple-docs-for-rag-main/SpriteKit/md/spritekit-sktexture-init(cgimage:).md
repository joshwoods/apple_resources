

- SpriteKit
- SKTexture
-  init(cgImage:) 

Initializer

# init(cgImage:)

Create a new texture object from a Quartz 2D image.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
convenience init(cgImage image: CGImage)
```

## Parameters 

`image`  

A Quartz 2D image (CGImage) object. For more information, see Quartz 2D Programming Guide and CGImage.

## Return Value

A new texture object.

## Discussion

The image data is copied before control is returned to your game.

## See Also

### Texture from Image

convenience init(image: UIImage)

Create a new texture object from an image object.

