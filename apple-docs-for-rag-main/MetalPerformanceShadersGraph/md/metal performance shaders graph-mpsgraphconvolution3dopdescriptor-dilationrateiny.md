

- Metal Performance Shaders Graph
- MPSGraphConvolution3DOpDescriptor
-  dilationRateInY 

Instance Property

# dilationRateInY

The amount by which weights tensor expands in the `y`-direction.

iOS 16.3+iPadOS 16.3+Mac Catalyst 16.3+macOS 13.2+tvOS 16.3+visionOS 1.0+

``` source
var dilationRateInY: Int { get set }
```

## Discussion

The weights tensor is dilated by inserting `dilationRateInY-1` zeros between consecutive values in `y`-dimension. Dilated weights tensor width is `(dilationRateInY-1)*kernelHeight+1`. Default value is 1.

