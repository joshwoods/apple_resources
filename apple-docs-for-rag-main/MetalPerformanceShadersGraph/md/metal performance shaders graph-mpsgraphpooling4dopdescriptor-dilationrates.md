

- Metal Performance Shaders Graph
- MPSGraphPooling4DOpDescriptor
-  dilationRates 

Instance Property

# dilationRates

Defines dilation rates for spatial dimensions. Must be four numbers, one for each spatial dimension, fastest running index last.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var dilationRates: [NSNumber] { get set }
```

## Discussion

Default value: `@[ @1, @1, @1, @1 ]`

