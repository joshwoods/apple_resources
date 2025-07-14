

- MetalKit
- MTKTextureLoader
-  newTexture(texture:options:) 

Instance Method

# newTexture(texture:options:)

Synchronously loads image data and creates a Metal texture from the specified Model I/O texture.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func newTexture(
    texture: MDLTexture,
    options: [MTKTextureLoader.Option : Any]? = nil
) throws -> any MTLTexture
```

## Parameters 

`texture`  

A Model I/O texture object containing image data from which to create the texture.

`options`  

A dictionary describing any additional texture loading steps. See `Texture Loading Options`.

## Return Value

A fully loaded and initialized Metal texture, or `nil` if an error occurred.

## See Also

### Loading Textures from Model I/O Representations

func newTexture(texture: MDLTexture, options: [MTKTextureLoader.Option : Any]?, completionHandler: MTKTextureLoader.Callback)

Asynchronously loads image data and creates a Metal texture from the specified Model I/O texture.

