

- MetalKit
- MTKTextureLoader
-  newTexture(name:scaleFactor:displayGamut:bundle:options:) 

Instance Method

# newTexture(name:scaleFactor:displayGamut:bundle:options:)

Synchronously loads image data and creates a Metal texture from the named texture asset in an asset catalog, using a specified display gamut.

macOS 10.12+

``` source
func newTexture(
    name: String,
    scaleFactor: CGFloat,
    displayGamut: NSDisplayGamut,
    bundle: Bundle?,
    options: [MTKTextureLoader.Option : Any]? = nil
) throws -> any MTLTexture
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

The resource bundle containing the asset catalog to load textures from.

`options`  

A dictionary describing any additional texture loading steps. See `Texture Loading Options`.

When using this method, the texture loader ignores the generateMipmaps, SRGB, cubeLayout, and origin options.

## Return Value

A fully loaded and initialized Metal texture, or `nil` if an error occurred.

## See Also

### Loading Textures from Asset Catalogs

func newTexture(name: String, scaleFactor: CGFloat, bundle: Bundle?, options: [MTKTextureLoader.Option : Any]?) throws -> any MTLTexture

Synchronously loads image data and creates a Metal texture from the named texture asset in an asset catalog.

func newTexture(name: String, scaleFactor: CGFloat, bundle: Bundle?, options: [MTKTextureLoader.Option : Any]?, completionHandler: MTKTextureLoader.Callback)

Asynchronously loads image data and creates a Metal texture from the named texture asset in an asset catalog.

func newTextures(names: [String], scaleFactor: CGFloat, bundle: Bundle?, options: [MTKTextureLoader.Option : Any]?, completionHandler: MTKTextureLoader.ArrayCallback)

Asynchronously loads image data and creates Metal textures from the specified list of named texture assets in an asset catalog.

func newTexture(name: String, scaleFactor: CGFloat, displayGamut: NSDisplayGamut, bundle: Bundle?, options: [MTKTextureLoader.Option : Any]?, completionHandler: MTKTextureLoader.Callback)

Asynchronously loads image data and creates a Metal texture from the named texture asset in an asset catalog.

func newTextures(names: [String], scaleFactor: CGFloat, displayGamut: NSDisplayGamut, bundle: Bundle?, options: [MTKTextureLoader.Option : Any]?, completionHandler: MTKTextureLoader.ArrayCallback)

Asynchronously loads image data and creates Metal textures from the specified list of named texture assets in an asset catalog.

