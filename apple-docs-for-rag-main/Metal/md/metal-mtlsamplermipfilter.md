

- Metal
-  MTLSamplerMipFilter 

Enumeration

# MTLSamplerMipFilter

Filtering options for determining what pixel value is returned with multiple mipmap levels.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
enum MTLSamplerMipFilter
```

## Topics

### Specifying Mip Filter Options

case notMipmapped

The texture is sampled from mipmap level `0`, and other mipmap levels are ignored.

case nearest

The nearest mipmap level is selected.

case linear

If the filter falls between mipmap levels, both levels are sampled and the results are determined by linear interpolation between levels.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var lodAverage: Bool

A Boolean value that specifies whether the GPU can use an average level of detail (LOD) when sampling from a texture.

var maxAnisotropy: Int

The number of samples that can be taken to improve the quality of sample footprints that are anisotropic.

enum MTLSamplerMinMagFilter

Filtering options for determining which pixel value is returned within a mipmap level.

