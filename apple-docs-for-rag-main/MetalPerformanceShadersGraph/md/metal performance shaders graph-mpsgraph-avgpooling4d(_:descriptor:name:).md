

- Metal Performance Shaders Graph
- MPSGraph
-  avgPooling4D(\_:descriptor:name:) 

Instance Method

# avgPooling4D(\_:descriptor:name:)

Creates a 4D average pooling operation and returns the result tensor.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func avgPooling4D(
    _ source: MPSGraphTensor,
    descriptor: MPSGraphPooling4DOpDescriptor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`source`  

A source tensor.

`descriptor`  

A pooling operation descriptor that specifies pooling window sizes, strides, dilation rates and paddings.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

