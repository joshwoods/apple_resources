

- MetalKit
- MTKTextureLoader
-  newTexture(URL:options:completionHandler:) 

Instance Method

# newTexture(URL:options:completionHandler:)

Asynchronously loads image data and creates a new Metal texture from a given URL.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func newTexture(
    URL: URL,
    options: [MTKTextureLoader.Option : Any]? = nil,
    completionHandler: @escaping MTKTextureLoader.Callback
)
```

``` source
func newTexture(
    URL: URL,
    options: [MTKTextureLoader.Option : Any]? = nil
) async throws -> any MTLTexture
```

## Parameters 

`URL`  

The URL of the file to load.

`options`  

A dictionary describing any additional texture loading steps. See `Texture Loading Options`.

`completionHandler`  

A block called when the texture has been loaded and fully initialized.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func newTexture(URL: URL, options: [MTKTextureLoader.Option : Any]? = nil) async throws -> MTLTexture
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Loading Textures from URLs

func newTexture(URL: URL, options: [MTKTextureLoader.Option : Any]?) throws -> any MTLTexture

Synchronously loads image data and creates a new Metal texture from a given URL.

func newTextures(URLs: [URL], options: [MTKTextureLoader.Option : Any]?, error: NSErrorPointer) -> [any MTLTexture]

Synchronously loads image data and creates new Metal textures from the specified list of URLs.

func newTextures(URLs: [URL], options: [MTKTextureLoader.Option : Any]?, completionHandler: MTKTextureLoader.ArrayCallback)

Asynchronously loads image data and creates new Metal textures from the specified list of URLs.

