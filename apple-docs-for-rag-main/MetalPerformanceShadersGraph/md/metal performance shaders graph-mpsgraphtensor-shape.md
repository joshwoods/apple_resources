

- Metal Performance Shaders Graph
- MPSGraphTensor
-  shape 

Instance Property

# shape

The shape of the tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var shape: [NSNumber]? { get }
```

## Discussion

Nil shape represents an unranked tensor. -1 value for a dimension represents that it will be resolved via shape inference at runtime and it can be anything.

