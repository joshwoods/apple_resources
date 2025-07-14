

- Metal Performance Shaders Graph
- MPSGraph
-  convolutionTranspose2D(\_:weights:outputShapeTensor:descriptor:name:) 

Instance Method

# convolutionTranspose2D(\_:weights:outputShapeTensor:descriptor:name:)

Creates a convolution transpose operation and returns the result tensor.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func convolutionTranspose2D(
    _ source: MPSGraphTensor,
    weights: MPSGraphTensor,
    outputShapeTensor outputShape: MPSGraphTensor,
    descriptor: MPSGraphConvolution2DOpDescriptor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`source`  

Input tensor

`weights`  

Weights tensor

`outputShape`  

1D Int32 or Int64 tensor. shape of the result tensor.

`descriptor`  

Descriptor for the corresponding forward Conv2D operation

`name`  

Name for the operation

## Return Value

A valid MPSGraphTensor object.

