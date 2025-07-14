

- Metal Performance Shaders Graph
- MPSGraphConvolution3DOpDescriptor
-  dilationRateInX 

Instance Property

# dilationRateInX

The amount by which weights tensor expands in the `x`-direction.

iOS 16.3+iPadOS 16.3+Mac Catalyst 16.3+macOS 13.2+tvOS 16.3+visionOS 1.0+

``` source
var dilationRateInX: Int { get set }
```

## Discussion

The weights tensor is dilated by inserting `dilationRateInX-1` zeros between consecutive values in `x`-dimension. Dilated weights tensor width is `(dilationRateInX-1)*kernelWidth+1`. Default value is 1.

