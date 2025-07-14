

- ML Compute
- MLCGraph
-  scatter(withDimension:source:indices:copyFrom:reductionType:) Deprecated

Instance Method

# scatter(withDimension:source:indices:copyFrom:reductionType:)

Adds a scatter layer to the graph.

iOS 14.5–17.4DeprecatediPadOS 14.5–17.4DeprecatedMac Catalyst 14.5–17.4DeprecatedmacOS 11.3–14.3DeprecatedtvOS 14.5–17.4Deprecated

``` source
func scatter(
    withDimension dimension: Int,
    source: MLCTensor,
    indices: MLCTensor,
    copyFrom: MLCTensor,
    reductionType: MLCReductionType
) -> MLCTensor?
```

## Parameters 

`dimension`  

The dimension along which to index.

`source`  

The source tensor.

`indices`  

The index of elements to scatter.

`copyFrom`  

The source tensor whose data is first copied to the result tensor.

`reductionType`  

The reduction type applied for all values in the source tensor that the system scatters to a specific location in the result tensor.

## Return Value

A scatter tensor.

## Discussion

The reductionType property must be MLCReductionType.none or MLCReductionType.sum.

## See Also

### Adding New Layers to Graphs

func split(source: MLCTensor, splitCount: Int, dimension: Int) -> [MLCTensor]?

Adds a new split layer to the graph using the source tensor, number of splits, and dimension to split the source tensor that you specify.

Deprecated

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

func transpose(dimensions: [Int], source: MLCTensor) -> MLCTensor?

Adds a new transpose layer to the graph using the dimensions and source tensor you specify.

Deprecated

