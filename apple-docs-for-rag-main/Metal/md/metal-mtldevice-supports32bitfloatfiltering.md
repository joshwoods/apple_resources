

- Metal
- MTLDevice
-  supports32BitFloatFiltering 

Instance Property

# supports32BitFloatFiltering

A Boolean value that indicates whether the GPU can filter a texture with a 32-bit floating-point format.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
var supports32BitFloatFiltering: Bool { get }
```

**Required**

## See Also

### Checking Texture and Sampler Support

var supportsBCTextureCompression: Bool

A Boolean value that indicates whether you can use textures that use BC compression.

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

