

- MetalKit
- MTKTextureLoader
-  newTexture(data:options:) 

Instance Method

# newTexture(data:options:)

Synchronously creates a new Metal texture from an in-memory representation of the texture’s data.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func newTexture(
    data: Data,
    options: [MTKTextureLoader.Option : Any]? = nil
) throws -> any MTLTexture
```

## Parameters 

`data`  

The NSData object containing image data.

`options`  

A dictionary describing any additional texture loading steps. See `Texture Loading Options`.

## Return Value

A fully loaded and initialized Metal texture, or `nil` if an error occurred.

## See Also

### Loading Textures from In-Memory Data Representations

func newTexture(data: Data, options: [MTKTextureLoader.Option : Any]?, completionHandler: MTKTextureLoader.Callback)

Asynchronously creates a new Metal texture from an in-memory representation of the texture’s data.

