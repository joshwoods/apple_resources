

- ML Compute
- MLCGraph
-  node(with:sources:) Deprecated

Instance Method

# node(with:sources:)

Adds the layer and source tensors that you specify to the graph.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
func node(
    with layer: MLCLayer,
    sources: [MLCTensor]
) -> MLCTensor?
```

## Parameters 

`layer`  

The layer.

`sources`  

An array that contains the source tensors.

## Return Value

A result tensor.

## See Also

### Adding Layers to Graphs

func node(with: MLCLayer, source: MLCTensor) -> MLCTensor?

Adds the layer and source tensor that you specify to the graph.

Deprecated

func node(with: MLCLayer, sources: [MLCTensor], disableUpdate: Bool) -> MLCTensor?

Adds the layer, source tensors, and option to disable optimizer updates that you specify to the graph.

Deprecated

func node(with: MLCLayer, sources: [MLCTensor], lossLabels: [MLCTensor]) -> MLCTensor?

Adds the layer, sources, and loss labels tensors that you specify to the graph.

Deprecated

