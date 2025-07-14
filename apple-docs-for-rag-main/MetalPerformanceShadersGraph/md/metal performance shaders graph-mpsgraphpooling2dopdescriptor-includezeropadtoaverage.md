

- Metal Performance Shaders Graph
- MPSGraphPooling2DOpDescriptor
-  includeZeroPadToAverage 

Instance Property

# includeZeroPadToAverage

Defines a mode for average pooling, where samples outside the input tensor count as zeroes in the average computation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var includeZeroPadToAverage: Bool { get set }
```

## Discussion

Otherwise the result is sum over samples divided by number of samples that didn’t come from padding. Default value: `NO`.

