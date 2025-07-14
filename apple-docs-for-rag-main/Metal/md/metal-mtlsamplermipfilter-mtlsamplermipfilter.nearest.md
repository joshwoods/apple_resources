

- Metal
- MTLSamplerMipFilter
-  MTLSamplerMipFilter.nearest 

Case

# MTLSamplerMipFilter.nearest

The nearest mipmap level is selected.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
case nearest
```

## See Also

### Specifying Mip Filter Options

case notMipmapped

The texture is sampled from mipmap level `0`, and other mipmap levels are ignored.

case linear

If the filter falls between mipmap levels, both levels are sampled and the results are determined by linear interpolation between levels.

