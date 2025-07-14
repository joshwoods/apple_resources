

- MetalKit
- MTKTextureLoader
-  newTextures(URLs:options:completionHandler:) 

Instance Method

# newTextures(URLs:options:completionHandler:)

Asynchronously loads image data and creates new Metal textures from the specified list of URLs.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func newTextures(
    URLs: [URL],
    options: [MTKTextureLoader.Option : Any]? = nil,
    completionHandler: @escaping MTKTextureLoader.ArrayCallback
)
```

``` source
func newTextures(
    URLs: [URL],
    options: [MTKTextureLoader.Option : Any]? = nil
) async throws -> [any MTLTexture]
```

## Parameters 

`URLs`  

An array of URLs referencing files to load.

`options`  

A dictionary describing any additional texture loading steps. See `Texture Loading Options`.

`completionHandler`  

A block called after all URLs have been processed. See the MTKTextureLoader.ArrayCallback signature to determine whether each texture has successfully loaded.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func newTextures(URLs: [URL], options: [MTKTextureLoader.Option : Any]? = nil) async throws -> [MTLTexture]
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Loading Textures from URLs

func newTexture(URL: URL, options: [MTKTextureLoader.Option : Any]?) throws -> any MTLTexture

Synchronously loads image data and creates a new Metal texture from a given URL.

func newTexture(URL: URL, options: [MTKTextureLoader.Option : Any]?, completionHandler: MTKTextureLoader.Callback)

Asynchronously loads image data and creates a new Metal texture from a given URL.

func newTextures(URLs: [URL], options: [MTKTextureLoader.Option : Any]?, error: NSErrorPointer) -> [any MTLTexture]

Synchronously loads image data and creates new Metal textures from the specified list of URLs.

