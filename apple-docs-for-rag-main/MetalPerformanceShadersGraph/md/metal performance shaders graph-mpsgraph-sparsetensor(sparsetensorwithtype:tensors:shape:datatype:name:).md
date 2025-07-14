

- Metal Performance Shaders Graph
- MPSGraph
-  sparseTensor(sparseTensorWithType:tensors:shape:dataType:name:) 

Instance Method

# sparseTensor(sparseTensorWithType:tensors:shape:dataType:name:)

Creates a sparse tensor representation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func sparseTensor(
    sparseTensorWithType sparseStorageType: MPSGraphSparseStorageType,
    tensors inputTensorArray: [MPSGraphTensor],
    shape: [NSNumber],
    dataType: MPSDataType,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`sparseStorageType`  

A sparseStorageType.

`inputTensorArray`  

An array of input tensors as \[sparseVals, indexTensor0, indexTensor1\].

`shape`  

The shape of the sparse tensor.

`dataType`  

The dataType of the sparse tensor.

`name`  

A name for the operation.

## Return Value

A valid MPSGraphTensor object.

## Discussion

sparseVals corresponds to non zero values in matrix. indexTensor0 and indexTensor1 are indices used for indexing into sparse data structure. For COO, indexTensor0 is x index and indexTensor1 is y index. For CSC, indexTensor0 and indexTensor1 correspond to rowIndex and colStarts respectively. For CSR, indexTensor0 and indexTensor1 correspond to colIndex and rowStarts respectively. You must set input tensors appropriately for each sparse storage type.

