

- Metal Performance Shaders Graph
- MPSGraph
-  avgPooling2DGradient(withGradientTensor:sourceTensor:descriptor:name:) 

Instance Method

# avgPooling2DGradient(withGradientTensor:sourceTensor:descriptor:name:)

Creates a 2D average pooling gradient operation and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func avgPooling2DGradient(
    withGradientTensor gradient: MPSGraphTensor,
    sourceTensor source: MPSGraphTensor,
    descriptor: MPSGraphPooling2DOpDescriptor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`gradient`  

A 2D input gradient tensor - must be of rank=4. The layout is defined by `descriptor.dataLayout`.

`source`  

The input tensor for the forward pass.

`descriptor`  

A pooling operation descriptor that specifies pooling window sizes, strides, dilation rates, paddings and layouts.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

