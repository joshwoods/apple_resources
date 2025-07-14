

- Metal
- MTLSamplerMinMagFilter
-  MTLSamplerMinMagFilter.linear 

Case

# MTLSamplerMinMagFilter.linear

Select two pixels in each dimension and interpolate linearly between them.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
case linear
```

## Discussion

Support for linear filtering varies by GPU and the format of the texture being sampled. For example, you can’t use linear filtering on textures with an integer format, and only some device objects support linear filtering for textures with a floating-point format. To determine whether linear filtering is available for a specific texture format, see:

- Metal feature set tables (PDF)

- Metal feature set tables (Numbers)

## See Also

### Filter options

case nearest

Select the single pixel nearest to the sample point.

