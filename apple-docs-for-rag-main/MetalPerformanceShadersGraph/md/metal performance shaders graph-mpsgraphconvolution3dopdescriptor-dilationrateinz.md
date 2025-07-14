

- Metal Performance Shaders Graph
- MPSGraphConvolution3DOpDescriptor
-  dilationRateInZ 

Instance Property

# dilationRateInZ

The amount by which weights tensor expands in the `z`-direction.

iOS 16.3+iPadOS 16.3+Mac Catalyst 16.3+macOS 13.2+tvOS 16.3+visionOS 1.0+

``` source
var dilationRateInZ: Int { get set }
```

## Discussion

The weights tensor is dilated by inserting `dilationRateInZ-1` zeros between consecutive values in `z`-dimension. Dilated weights tensor depth is `(dilationRateInZ-1)*kernelDepth+1`. Default value is 1.

