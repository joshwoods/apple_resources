

- Metal Performance Shaders Graph
- MPSGraph
-  gatherND(withUpdatesTensor:indicesTensor:batchDimensions:name:) 

Instance Method

# gatherND(withUpdatesTensor:indicesTensor:batchDimensions:name:)

Creates a GatherND operation and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func gatherND(
    withUpdatesTensor updatesTensor: MPSGraphTensor,
    indicesTensor: MPSGraphTensor,
    batchDimensions: Int,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`updatesTensor`  

Tensor containing slices to be inserted into the result tensor.

`indicesTensor`  

Tensor containg the updates indices to read slices from

`batchDimensions`  

The number of batch dimensions

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

## Discussion

Gathers the slices in updatesTensor to the result tensor along the indices in indicesTensor. The gather is defined as

```
B = batchDims 
U = updates.rank - B 
P = res.rank - B 
Q = inds.rank - B 
K = inds.shape[-1] 
index_slice = indices[i_{b0},...,i_{bB},i_{0},..,i_{Q-1}] 
res[i_{b0},...,i_{bB},i_{0},...,i_{Q-1}] = updates[i_{b0},...,i_{bB},index_slice[0],...,index_slice[K-1]] 
```

The tensors have the following shape requirements

```
U > 0; P > 0; Q > 0 
K 

