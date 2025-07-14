

- MetalKit
- MTKTextureLoader
- MTKTextureLoader.Option
-  cubeLayout 

Type Property

# cubeLayout

A key used to specify how cube texture data is arranged in the source image.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
static let cubeLayout: MTKTextureLoader.Option
```

## Discussion

The value for this key is one of the values listed for MTKTextureLoader.CubeLayout. If this option is omitted, the texture loader does not create a cube texture.

This option cannot be used with PVR files, KTX files, or MDLTexture objects, which support cube textures directly.

## See Also

### Specifying Cube Layout

struct CubeLayout

Options for specifying how cube texture data is arranged in the source image.

