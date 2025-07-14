

- MetalKit
- MTKTextureLoader
- MTKTextureLoader.Option
-  generateMipmaps 

Type Property

# generateMipmaps

A key used to specify whether the texture loader should generate mipmaps for the texture.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
static let generateMipmaps: MTKTextureLoader.Option
```

## Discussion

The value for this key is an NSNumber object containing a boolean value.

If the value is true, the resulting texture will be created with mipmaps. If the file being loaded contains data for mipmaps (such as in a PVR or KTX file), specifying this option will overwrite the existing mipmap data in the loaded texture.

This option can be used only if the pixel format of the texture is filterable and color-renderable; see the Pixel Format Capabilities for more information.

This option also implies that allocateMipmaps is true. Specifying this option causes the MTKTextureLoader object to submit work to the GPU on your behalf.

## See Also

### Specifying Mipmap Options

static let allocateMipmaps: MTKTextureLoader.Option

A key used to specify whether the texture loader should allocate memory for mipmaps in the texture.

