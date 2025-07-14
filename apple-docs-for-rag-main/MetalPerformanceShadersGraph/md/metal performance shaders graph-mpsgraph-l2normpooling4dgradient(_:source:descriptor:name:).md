

- Metal Performance Shaders Graph
- MPSGraph
-  L2NormPooling4DGradient(\_:source:descriptor:name:) 

Instance Method

# L2NormPooling4DGradient(\_:source:descriptor:name:)

Creates a L2-Norm pooling gradient operation and returns the result tensor.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func L2NormPooling4DGradient(
    _ gradient: MPSGraphTensor,
    source: MPSGraphTensor,
    descriptor: MPSGraphPooling4DOpDescriptor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`gradient`  

An input gradient tensor.

`source`  

The input tensor for the forward pass.

`descriptor`  

A pooling operation descriptor that specifies pooling window sizes, strides, dilation rates and paddings.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

