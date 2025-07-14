

- SpriteKit
- SKTexture
-  init(data:size:flipped:) 

Initializer

# init(data:size:flipped:)

Creates a new texture from raw pixel data.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
convenience init(
    data pixelData: Data,
    size: CGSize,
    flipped: Bool
)
```

## Parameters 

`pixelData`  

An `NSData` object that holds the bitmap data. The pixels must be 32 bpp, 8bpc (unsigned integer) RGBA pixel data. The color components should have been already multiplied by the alpha value.

`size`  

The size of the new texture in points.

`flipped`  

A Boolean value that indicates whether the image data should be vertically flipped before creating the texture.

## Return Value

A new texture object.

## Discussion

The image data is copied before control is returned to your game.

## See Also

### Texture from Data

convenience init(data: Data, size: CGSize)

Creates a new texture from raw pixel data.

convenience init(data: Data, size: CGSize, rowLength: UInt32, alignment: UInt32)

Creates a new texture from custom formatted raw pixel data.

