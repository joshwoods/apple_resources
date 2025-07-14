

- ML Compute
- MLCGraph
-  split(source:splitCount:dimension:) Deprecated

Instance Method

# split(source:splitCount:dimension:)

Adds a new split layer to the graph using the source tensor, number of splits, and dimension to split the source tensor that you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
func split(
    source: MLCTensor,
    splitCount: Int,
    dimension: Int
) -> [MLCTensor]?
```

## Parameters 

`source`  

The source tensor.

`splitCount`  

The number of splits.

`dimension`  

The dimension along which to split the tensor.

## Return Value

A result tensor.

## See Also

### Adding New Layers to Graphs

func split(source: MLCTensor, splitSectionLengths: [Int], dimension: Int) -> [MLCTensor]?

Adds a new split layer to the graph using the source tensor, lengths of each split section, and dimension to split the source tensor that you specify.

Deprecated

func concatenate(sources: [MLCTensor], dimension: Int) -> MLCTensor?

Adds a new concatenation layer to the graph using the source tensors and concatenation dimension you specify.

Deprecated

func reshape(shape: [Int], source: MLCTensor) -> MLCTensor?

Adds a new reshape layer to the graph using the shape and source tensor you specify.

Deprecated

func gather(withDimension: Int, source: MLCTensor, indices: MLCTensor) -> MLCTensor?

Adds a gather layer to the graph using the source tensor, dimension along which to index, and the indices you specify.

Deprecated

func scatter(withDimension: Int, source: MLCTensor, indices: MLCTensor, copyFrom: MLCTensor, reductionType: MLCReductionType) -> MLCTensor?

Adds a scatter layer to the graph.

Deprecated

func transpose(dimensions: [Int], source: MLCTensor) -> MLCTensor?

Adds a new transpose layer to the graph using the dimensions and source tensor you specify.

Deprecated

