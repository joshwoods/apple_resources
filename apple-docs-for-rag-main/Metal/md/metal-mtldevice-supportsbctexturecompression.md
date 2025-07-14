

- Metal
- MTLDevice
-  supportsBCTextureCompression 

Instance Property

# supportsBCTextureCompression

A Boolean value that indicates whether you can use textures that use BC compression.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 11.0+tvOS 16.4+visionOS 1.0+

``` source
var supportsBCTextureCompression: Bool { get }
```

**Required**

## See Also

### Checking Texture and Sampler Support

var supports32BitFloatFiltering: Bool

A Boolean value that indicates whether the GPU can filter a texture with a 32-bit floating-point format.

**Required**

var isDepth24Stencil8PixelFormatSupported: Bool

A Boolean value that indicates whether a device supports a packed depth-and-stencil pixel format.

**Required**

var supportsQueryTextureLOD: Bool

A Boolean value that indicates whether you can query the texture level of detail from within a shader.

**Required**

var readWriteTextureSupport: MTLReadWriteTextureTier

The GPU device’s texture support tier.

**Required**

