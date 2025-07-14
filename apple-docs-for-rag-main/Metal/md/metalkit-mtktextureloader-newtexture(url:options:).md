

- MetalKit
- MTKTextureLoader
-  newTexture(URL:options:) 

Instance Method

# newTexture(URL:options:)

Synchronously loads image data and creates a new Metal texture from a given URL.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func newTexture(
    URL: URL,
    options: [MTKTextureLoader.Option : Any]? = nil
) throws -> any MTLTexture
```

## Parameters 

`URL`  

The URL of the file to load.

`options`  

A dictionary describing any additional texture loading steps. See `Texture Loading Options`.

## Return Value

A fully loaded and initialized Metal texture, or `nil` if an error occurred.

## See Also

### Loading Textures from URLs

func newTexture(URL: URL, options: [MTKTextureLoader.Option : Any]?, completionHandler: MTKTextureLoader.Callback)

Asynchronously loads image data and creates a new Metal texture from a given URL.

func newTextures(URLs: [URL], options: [MTKTextureLoader.Option : Any]?, error: NSErrorPointer) -> [any MTLTexture]

Synchronously loads image data and creates new Metal textures from the specified list of URLs.

func newTextures(URLs: [URL], options: [MTKTextureLoader.Option : Any]?, completionHandler: MTKTextureLoader.ArrayCallback)

Asynchronously loads image data and creates new Metal textures from the specified list of URLs.

