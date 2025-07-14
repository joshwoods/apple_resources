

- ML Compute
- MLCGraph
-  transpose(dimensions:source:) Deprecated

Instance Method

# transpose(dimensions:source:)

Adds a new transpose layer to the graph using the dimensions and source tensor you specify.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0Deprecated

``` source
func transpose(
    dimensions: [Int],
    source: MLCTensor
) -> MLCTensor?
```

Deprecated

Use Metal Performance Shaders Graph or BNNS instead.

## Parameters 

`dimensions`  

An array that contains the desired ordering of dimensions.

`source`  

The source tensor.

## Return Value

A result tensor.

## Discussion

The dimensions array specifies the input axis source for each output axis. In other words, the `n`th element in the dimensions array specifies the input axis source for the `n`th axis in the output.

Note

The batch dimension is typically axis 0, which you can’t transpose.

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

func scatter(withDimension: Int, source: MLCTensor, indices: MLCTensor, copyFrom: MLCTensor, reductionType: MLCReductionType) -> MLCTensor?

Adds a scatter layer to the graph.

Deprecated

