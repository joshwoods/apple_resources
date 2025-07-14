

- Metal
- MTLDevice
-  isDepth24Stencil8PixelFormatSupported 

Instance Property

# isDepth24Stencil8PixelFormatSupported

A Boolean value that indicates whether a device supports a packed depth-and-stencil pixel format.

Mac Catalyst 13.0+macOS 10.11+

``` source
var isDepth24Stencil8PixelFormatSupported: Bool { get }
```

**Required**

## Discussion

If the value is true, the device supports the MTLPixelFormat.depth24Unorm_stencil8 pixel format.

## See Also

### Related Documentation

Metal Shading Language Guide

Metal Programming Guide

### Checking Texture and Sampler Support

var supports32BitFloatFiltering: Bool

A Boolean value that indicates whether the GPU can filter a texture with a 32-bit floating-point format.

**Required**

var supportsBCTextureCompression: Bool

A Boolean value that indicates whether you can use textures that use BC compression.

**Required**

var supportsQueryTextureLOD: Bool

A Boolean value that indicates whether you can query the texture level of detail from within a shader.

**Required**

var readWriteTextureSupport: MTLReadWriteTextureTier

The GPU device’s texture support tier.

**Required**

