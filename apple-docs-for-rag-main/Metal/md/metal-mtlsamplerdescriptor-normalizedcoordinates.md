

- Metal
- MTLSamplerDescriptor
-  normalizedCoordinates 

Instance Property

# normalizedCoordinates

A Boolean value that indicates whether texture coordinates are normalized to the range `[0.0, 1.0]`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var normalizedCoordinates: Bool { get set }
```

## Discussion

If true, texture coordinates are from `0.0` to `1.0`. If false, texture coordinates are from `0` to `width` for horizontal coordinates and `0` to `height` for vertical coordinates. The default value is true.

Non-normalized texture coordinates should only be used with 1D and 2D textures with the following conditions; otherwise, the results of sampling are undefined.

- The MTLSamplerAddressMode.clampToEdge or MTLSamplerAddressMode.clampToZero address mode.

- The MTLSamplerMipFilter.notMipmapped mipmap filtering option.

- minFilter and magFilter must be equal to each other.

- maxAnisotropy must be `1`.

