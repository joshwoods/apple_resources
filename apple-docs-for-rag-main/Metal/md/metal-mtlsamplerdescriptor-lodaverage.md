

- Metal
- MTLSamplerDescriptor
-  lodAverage 

Instance Property

# lodAverage

A Boolean value that specifies whether the GPU can use an average level of detail (LOD) when sampling from a texture.

iOS 9.0+iPadOS 9.0+Mac Catalyst 14.0+macOS 11.0+tvOS 9.0+visionOS 1.0+

``` source
var lodAverage: Bool { get set }
```

## Discussion

If this value is true, an average LOD may be used across four fragment shader threads. If this value is false, no averaging is performed and each thread accesses its own LOD.

The default value is false.

Note

This optional Boolean value is used as a performance optimization hint and it is ignored on some GPUs. Enabling LOD averaging may provide a performance benefit for shaders that sample from explicit per-fragment mipmap levels, or apply per-fragment LOD bias, at the potential cost of reduced texture sample quality.

## See Also

### Declaring Filter Modes

var minFilter: MTLSamplerMinMagFilter

The filtering option for combining pixels within one mipmap level when the sample footprint is larger than a pixel (minification).

var magFilter: MTLSamplerMinMagFilter

The filtering operation for combining pixels within one mipmap level when the sample footprint is smaller than a pixel (magnification).

var mipFilter: MTLSamplerMipFilter

The filtering option for combining pixels between two mipmap levels.

var lodMinClamp: Float

The minimum level of detail (LOD) to use when sampling from a texture.

var lodMaxClamp: Float

The maximum level of detail (LOD) to use when sampling from a texture.

var maxAnisotropy: Int

The number of samples that can be taken to improve the quality of sample footprints that are anisotropic.

enum MTLSamplerMinMagFilter

Filtering options for determining which pixel value is returned within a mipmap level.

enum MTLSamplerMipFilter

Filtering options for determining what pixel value is returned with multiple mipmap levels.

