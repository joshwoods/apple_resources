

- MetalKit
- MTKTextureLoader
-  newTexture(cgImage:options:completionHandler:) 

Instance Method

# newTexture(cgImage:options:completionHandler:)

Asynchronously loads image data and creates a new Metal texture from a given bitmap image.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func newTexture(
    cgImage: CGImage,
    options: [MTKTextureLoader.Option : Any]? = nil,
    completionHandler: @escaping MTKTextureLoader.Callback
)
```

``` source
func newTexture(
    cgImage: CGImage,
    options: [MTKTextureLoader.Option : Any]? = nil
) async throws -> any MTLTexture
```

## Parameters 

`cgImage`  

The CGImage from which to load image data.

`options`  

A dictionary describing any additional texture loading steps. See `Texture Loading Options`.

`completionHandler`  

A block called when the texture has been loaded and fully initialized.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func newTexture(cgImage: CGImage, options: [MTKTextureLoader.Option : Any]? = nil) async throws -> MTLTexture
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Loading Textures from Core Graphics Images

func newTexture(cgImage: CGImage, options: [MTKTextureLoader.Option : Any]?) throws -> any MTLTexture

Synchronously loads image data and creates a new Metal texture from a given bitmap image.

