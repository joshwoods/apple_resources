

- Metal Performance Shaders Graph
- MPSGraphConvolution2DOpDescriptor
-  dilationRateInX 

Instance Property

# dilationRateInX

The amount by which the weights tensor expands in the `x`-direction.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var dilationRateInX: Int { get set }
```

## Discussion

The weights tensor is dilated by inserting `dilationRateInX-1` zeros between consecutive values in `x`-dimension. Dilated weights tensor width is `(dilationRateInX-1)*kernelWidth+1`. Default value is 1.

