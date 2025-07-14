

- Metal Performance Shaders Graph
- MPSGraphPooling4DOpDescriptor
-  kernelSizes 

Instance Property

# kernelSizes

Defines the pooling window size.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var kernelSizes: [NSNumber] { get set }
```

## Discussion

Must be four numbers, one for each spatial dimension, fastest running index last.

