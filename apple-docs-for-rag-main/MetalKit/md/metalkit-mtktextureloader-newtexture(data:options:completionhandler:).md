

- MetalKit
- MTKTextureLoader
-  newTexture(data:options:completionHandler:) 

Instance Method

# newTexture(data:options:completionHandler:)

Asynchronously creates a new Metal texture from an in-memory representation of the texture’s data.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func newTexture(
    data: Data,
    options: [MTKTextureLoader.Option : Any]? = nil,
    completionHandler: @escaping MTKTextureLoader.Callback
)
```

``` source
func newTexture(
    data: Data,
    options: [MTKTextureLoader.Option : Any]? = nil
) async throws -> any MTLTexture
```

## Parameters 

`data`  

The NSData object containing image data.

`options`  

A dictionary describing any additional texture loading steps. See `Texture Loading Options`.

`completionHandler`  

A block called when the texture has been loaded and fully initialized.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func newTexture(data: Data, options: [MTKTextureLoader.Option : Any]? = nil) async throws -> MTLTexture
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Loading Textures from In-Memory Data Representations

func newTexture(data: Data, options: [MTKTextureLoader.Option : Any]?) throws -> any MTLTexture

Synchronously creates a new Metal texture from an in-memory representation of the texture’s data.

