

- Metal Performance Shaders Graph
- MPSGraph
-  scatterAlongAxis(\_:data:updates:indices:mode:name:) 

Instance Method

# scatterAlongAxis(\_:data:updates:indices:mode:name:)

Creates a ScatterAlongAxis operation and returns the result tensor.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+

``` source
func scatterAlongAxis(
    _ axis: Int,
    data dataTensor: MPSGraphTensor,
    updates updatesTensor: MPSGraphTensor,
    indices indicesTensor: MPSGraphTensor,
    mode: MPSGraphScatterMode,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`axis`  

The axis to scatter to. Negative values wrap around

`dataTensor`  

The input tensor to scatter values onto

`updatesTensor`  

The input tensor to scatter values from

`indicesTensor`  

Int32 or Int64 tensor used to index the result tensor.

`mode`  

The type of update to use

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

## Discussion

Scatter values from `updatesTensor` along the specified `axis` at indices in `indicesTensor` onto `dataTensor`. Values in `dataTensor` are updated following `mode`. See MPSGraphScatterMode. The shape of `updatesTensor` and `indicesTensor` must match. The shape of `dataTensor` must match except at `axis`. If an index is out of bounds of `shape` along `axis` the update value is skipped. For example,

```
data = [ [0, 0, 0],
         [1, 1, 1],
         [2, 2, 2],
         [3, 3, 3] ]
updates = [ [1, 2, 3],
            [4, 5, 6] ]
indices = [ [2, 1, 0],
            [1, 3, 2] ]
axis = 0
result = scatterAlongAxis(axis, data, updates, indices, MPSGraphScatterModeAdd, "scatter")
result = [ [0, 0, 3],
           [5, 3, 1],
           [3, 2, 8],
           [3, 8, 3] ]
```

