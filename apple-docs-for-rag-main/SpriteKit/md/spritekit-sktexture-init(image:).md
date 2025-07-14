

- SpriteKit
- SKTexture
-  init(image:) 

Initializer

# init(image:)

Create a new texture object from an image object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
convenience init(image: UIImage)
```

**macOS**

``` source
convenience init(image: NSImage)
```

## Parameters 

`image`  

An image.

## Return Value

A new texture object.

## Discussion

The image data is copied before control is returned to your game.

## See Also

### Texture from Image

convenience init(cgImage: CGImage)

Create a new texture object from a Quartz 2D image.

