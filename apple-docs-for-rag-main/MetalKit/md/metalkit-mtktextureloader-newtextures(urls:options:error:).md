

- MetalKit
- MTKTextureLoader
-  newTextures(URLs:options:error:) 

Instance Method

# newTextures(URLs:options:error:)

Synchronously loads image data and creates new Metal textures from the specified list of URLs.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func newTextures(
    URLs: [URL],
    options: [MTKTextureLoader.Option : Any]? = nil,
    error: NSErrorPointer
) -> [any MTLTexture]
```

## Parameters 

`URLs`  

An array of URLs referencing files to load.

`options`  

A dictionary describing any additional texture loading steps. See `Texture Loading Options`.

`error`  

If all textures were fully loaded and initialized, this pointer is `nil` on output. If an error occurs while loading any of the specified URLs, this pointer refers to an NSError object describing the failure. (Which element in the `URLs` array the error corresponds to is undefined.)

## Return Value

An array of Metal textures, each corresponding to a URL listed in the `URLs` parameter. If an error occurs while loading a texture, the corresponding array element is an NSNull object.

## See Also

### Loading Textures from URLs

func newTexture(URL: URL, options: [MTKTextureLoader.Option : Any]?) throws -> any MTLTexture

Synchronously loads image data and creates a new Metal texture from a given URL.

func newTexture(URL: URL, options: [MTKTextureLoader.Option : Any]?, completionHandler: MTKTextureLoader.Callback)

Asynchronously loads image data and creates a new Metal texture from a given URL.

func newTextures(URLs: [URL], options: [MTKTextureLoader.Option : Any]?, completionHandler: MTKTextureLoader.ArrayCallback)

Asynchronously loads image data and creates new Metal textures from the specified list of URLs.

