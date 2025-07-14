

- Metal Performance Shaders Graph
- MPSGraphDepthwiseConvolution3DOpDescriptor
-  dilationRates 

Instance Property

# dilationRates

The dilation rates for spatial dimensions.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var dilationRates: [NSNumber] { get set }
```

## Discussion

Must be three numbers, one for each spatial dimension, fastest running index last. Default value: `@[ @1, @1, @1 ]`

