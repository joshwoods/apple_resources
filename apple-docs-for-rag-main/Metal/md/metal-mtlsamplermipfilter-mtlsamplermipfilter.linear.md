

- Metal
- MTLSamplerMipFilter
-  MTLSamplerMipFilter.linear 

Case

# MTLSamplerMipFilter.linear

If the filter falls between mipmap levels, both levels are sampled and the results are determined by linear interpolation between levels.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
case linear
```

## Discussion

Support for linear filtering between mipmaps varies by GPU and the format of the texture being sampled. For example, you can’t use linear filtering on textures with an integer format, and only some device objects support linear filtering for textures with a floating-point format. To determine whether linear filtering is available for a specific texture format, see:

- Metal feature set tables (PDF)

- Metal feature set tables (Numbers)

## See Also

### Specifying Mip Filter Options

case notMipmapped

The texture is sampled from mipmap level `0`, and other mipmap levels are ignored.

case nearest

The nearest mipmap level is selected.

