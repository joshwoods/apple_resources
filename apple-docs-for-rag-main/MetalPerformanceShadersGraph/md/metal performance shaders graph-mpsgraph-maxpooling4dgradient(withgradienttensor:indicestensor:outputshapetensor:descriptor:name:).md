

- Metal Performance Shaders Graph
- MPSGraph
-  maxPooling4DGradient(withGradientTensor:indicesTensor:outputShapeTensor:descriptor:name:) 

Instance Method

# maxPooling4DGradient(withGradientTensor:indicesTensor:outputShapeTensor:descriptor:name:)

Creates a max-pooling gradient operation and returns the result tensor.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func maxPooling4DGradient(
    withGradientTensor gradient: MPSGraphTensor,
    indicesTensor indices: MPSGraphTensor,
    outputShapeTensor outputShape: MPSGraphTensor,
    descriptor: MPSGraphPooling4DOpDescriptor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`gradient`  

An input gradient tensor.

`indices`  

The indices tensor returned from maxPooling4DReturnIndices(_:descriptor:name:).

`outputShape`  

A tensor containing the shape of the destination gradient.

`descriptor`  

A pooling operation descriptor that specifies pooling window sizes, strides, dilation rates, paddings and layouts.

`name`  

The name for the operation.

## Return Value

Destination gradient tensor.

## Discussion

With this API MPSGraph computes the max-pooling gradient efficiently by reusing the indices from the forward API instead of recomputing them. The descriptor must set `returnIndicesMode` and `returnIndicesDataType` to the same value as that set by the forward pass.

