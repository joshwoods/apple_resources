

- Metal Performance Shaders Graph
- MPSGraph
-  stencil(withSourceTensor:weightsTensor:descriptor:name:) 

Instance Method

# stencil(withSourceTensor:weightsTensor:descriptor:name:)

Creates a stencil operation and returns the result tensor.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func stencil(
    withSourceTensor source: MPSGraphTensor,
    weightsTensor weights: MPSGraphTensor,
    descriptor: MPSGraphStencilOpDescriptor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`source`  

The tensor containing the source data. Must be of rank 4 or greater.

`weights`  

A 4-D tensor containing the weights data.

`descriptor`  

The descriptor object that specifies the parameters for the stencil operation.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

## Discussion

Performs a weighted reduction operation (See reductionMode) on the last 4 dimensions of the `source` over the window determined by `weights`, according to the value defined in `descriptor`.

```
   y[i] = reduction{j \in w} ( x[ i + j ]w[j] )
```

