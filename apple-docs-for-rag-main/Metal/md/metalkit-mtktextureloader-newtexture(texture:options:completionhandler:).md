

- MetalKit
- MTKTextureLoader
-  newTexture(texture:options:completionHandler:) 

Instance Method

# newTexture(texture:options:completionHandler:)

Asynchronously loads image data and creates a Metal texture from the specified Model I/O texture.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func newTexture(
    texture: MDLTexture,
    options: [MTKTextureLoader.Option : Any]? = nil,
    completionHandler: @escaping MTKTextureLoader.Callback
)
```

``` source
func newTexture(
    texture: MDLTexture,
    options: [MTKTextureLoader.Option : Any]? = nil
) async throws -> any MTLTexture
```

## Parameters 

`texture`  

A Model I/O texture object containing image data from which to create the texture.

`options`  

A dictionary describing any additional texture loading steps. See `Texture Loading Options`.

`completionHandler`  

A block called when the texture has been loaded and fully initialized.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func newTexture(texture: MDLTexture, options: [MTKTextureLoader.Option : Any]? = nil) async throws -> MTLTexture
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Loading Textures from Model I/O Representations

func newTexture(texture: MDLTexture, options: [MTKTextureLoader.Option : Any]?) throws -> any MTLTexture

Synchronously loads image data and creates a Metal texture from the specified Model I/O texture.

