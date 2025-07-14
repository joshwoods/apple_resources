

- MetalKit
- MTKTextureLoader
-  newTexture(name:scaleFactor:displayGamut:bundle:options:completionHandler:) 

Instance Method

# newTexture(name:scaleFactor:displayGamut:bundle:options:completionHandler:)

Asynchronously loads image data and creates a Metal texture from the named texture asset in an asset catalog.

macOS 10.12+

``` source
func newTexture(
    name: String,
    scaleFactor: CGFloat,
    displayGamut: NSDisplayGamut,
    bundle: Bundle?,
    options: [MTKTextureLoader.Option : Any]? = nil,
    completionHandler: @escaping MTKTextureLoader.Callback
)
```

``` source
func newTexture(
    name: String,
    scaleFactor: CGFloat,
    displayGamut: NSDisplayGamut,
    bundle: Bundle?,
    options: [MTKTextureLoader.Option : Any]? = nil
) async throws -> any MTLTexture
```

## Parameters 

`name`  

The name of a texture in an asset catalog.

`scaleFactor`  

The scale factor of texture to request.

In iOS and tvOS, pass the contentsScale value of the view where you plan to display texture content.

In macOS, pass the backingScaleFactor value of the window where you plan to display texture content.

`displayGamut`  

The version of the texture based on the *Gamut* trait in Xcode.

To determine the appropriate parameter value, pass the widest `NSDisplayGamut` value that returns true when queried against the `canRepresentDisplayGamut:` method of `NSWindow`.

`bundle`  

The resource bundle containing the asset catalog to load the texture from.

`options`  

A dictionary describing any additional texture loading steps. See `Texture Loading Options`.

When using this method, the texture loader ignores the generateMipmaps, SRGB, cubeLayout, and origin options.

`completionHandler`  

A block called when the texture has been loaded and fully initialized.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func newTexture(name: String, scaleFactor: CGFloat, displayGamut: NSDisplayGamut, bundle: Bundle?, options: [MTKTextureLoader.Option : Any]? = nil) async throws -> MTLTexture
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Loading Textures from Asset Catalogs

func newTexture(name: String, scaleFactor: CGFloat, bundle: Bundle?, options: [MTKTextureLoader.Option : Any]?) throws -> any MTLTexture

Synchronously loads image data and creates a Metal texture from the named texture asset in an asset catalog.

func newTexture(name: String, scaleFactor: CGFloat, bundle: Bundle?, options: [MTKTextureLoader.Option : Any]?, completionHandler: MTKTextureLoader.Callback)

Asynchronously loads image data and creates a Metal texture from the named texture asset in an asset catalog.

func newTextures(names: [String], scaleFactor: CGFloat, bundle: Bundle?, options: [MTKTextureLoader.Option : Any]?, completionHandler: MTKTextureLoader.ArrayCallback)

Asynchronously loads image data and creates Metal textures from the specified list of named texture assets in an asset catalog.

func newTexture(name: String, scaleFactor: CGFloat, displayGamut: NSDisplayGamut, bundle: Bundle?, options: [MTKTextureLoader.Option : Any]?) throws -> any MTLTexture

Synchronously loads image data and creates a Metal texture from the named texture asset in an asset catalog, using a specified display gamut.

func newTextures(names: [String], scaleFactor: CGFloat, displayGamut: NSDisplayGamut, bundle: Bundle?, options: [MTKTextureLoader.Option : Any]?, completionHandler: MTKTextureLoader.ArrayCallback)

Asynchronously loads image data and creates Metal textures from the specified list of named texture assets in an asset catalog.

