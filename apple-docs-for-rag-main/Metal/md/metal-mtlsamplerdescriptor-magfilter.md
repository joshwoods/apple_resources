

- Metal
- MTLSamplerDescriptor
-  magFilter 

Instance Property

# magFilter

The filtering operation for combining pixels within one mipmap level when the sample footprint is smaller than a pixel (magnification).

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var magFilter: MTLSamplerMinMagFilter { get set }
```

## Mentioned in 

Improving CPU Performance by Using Argument Buffers

## Discussion

The default value is MTLSamplerMinMagFilter.nearest.

## See Also

### Declaring Filter Modes

var minFilter: MTLSamplerMinMagFilter

The filtering option for combining pixels within one mipmap level when the sample footprint is larger than a pixel (minification).

var mipFilter: MTLSamplerMipFilter

The filtering option for combining pixels between two mipmap levels.

var lodMinClamp: Float

The minimum level of detail (LOD) to use when sampling from a texture.

var lodMaxClamp: Float

The maximum level of detail (LOD) to use when sampling from a texture.

var lodAverage: Bool

A Boolean value that specifies whether the GPU can use an average level of detail (LOD) when sampling from a texture.

var maxAnisotropy: Int

The number of samples that can be taken to improve the quality of sample footprints that are anisotropic.

enum MTLSamplerMinMagFilter

Filtering options for determining which pixel value is returned within a mipmap level.

enum MTLSamplerMipFilter

Filtering options for determining what pixel value is returned with multiple mipmap levels.

