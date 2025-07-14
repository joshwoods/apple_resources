

- Metal Performance Shaders Graph
- MPSGraph
-  oneHot(withIndicesTensor:depth:name:) 

Instance Method

# oneHot(withIndicesTensor:depth:name:)

Creates a oneHot operation and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func oneHot(
    withIndicesTensor indicesTensor: MPSGraphTensor,
    depth: Int,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`indicesTensor`  

Tensor of indices for on values

`depth`  

Depth of the oneHot vector along the axis

`name`  

Name for the operation

## Return Value

A valid MPSGraphTensor object.

## Discussion

Creates a tensor of rank equal to the rank of `indicesTensor` + 1, of type MPSDataTypeFloat32. Inserts a new axis at the minor dimension. The values at the indices in the indicesTensor will be set to 1, and all other values will be set to 0.

