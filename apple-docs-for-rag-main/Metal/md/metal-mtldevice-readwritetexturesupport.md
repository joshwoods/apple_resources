

- Metal
- MTLDevice
-  readWriteTextureSupport 

Instance Property

# readWriteTextureSupport

The GPU device’s texture support tier.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var readWriteTextureSupport: MTLReadWriteTextureTier { get }
```

**Required**

## Topics

### Read-Write Texture Tiers

enum MTLReadWriteTextureTier

The support level for read-write texture formats.

## See Also

### Checking Texture and Sampler Support

var supports32BitFloatFiltering: Bool

A Boolean value that indicates whether the GPU can filter a texture with a 32-bit floating-point format.

**Required**

var supportsBCTextureCompression: Bool

A Boolean value that indicates whether you can use textures that use BC compression.

**Required**

var isDepth24Stencil8PixelFormatSupported: Bool

A Boolean value that indicates whether a device supports a packed depth-and-stencil pixel format.

**Required**

var supportsQueryTextureLOD: Bool

A Boolean value that indicates whether you can query the texture level of detail from within a shader.

**Required**

