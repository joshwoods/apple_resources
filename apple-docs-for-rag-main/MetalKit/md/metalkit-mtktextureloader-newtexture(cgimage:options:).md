

- MetalKit
- MTKTextureLoader
-  newTexture(cgImage:options:) 

Instance Method

# newTexture(cgImage:options:)

Synchronously loads image data and creates a new Metal texture from a given bitmap image.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func newTexture(
    cgImage: CGImage,
    options: [MTKTextureLoader.Option : Any]? = nil
) throws -> any MTLTexture
```

## Parameters 

`cgImage`  

The CGImage from which to load image data.

`options`  

A dictionary describing any additional texture loading steps. See `Texture Loading Options`.

## Return Value

A fully loaded and initialized Metal texture, or `nil` if an error occurred.

## See Also

### Loading Textures from Core Graphics Images

func newTexture(cgImage: CGImage, options: [MTKTextureLoader.Option : Any]?, completionHandler: MTKTextureLoader.Callback)

Asynchronously loads image data and creates a new Metal texture from a given bitmap image.

