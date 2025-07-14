

- ML Compute
- MLCGraph
-  sourceTensors(for:) Deprecated

Instance Method

# sourceTensors(for:)

Gets the source tensors for a layer in the training graph.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
func sourceTensors(for layer: MLCLayer) -> [MLCTensor]
```

## Parameters 

`layer`  

A layer in the training graph.

## Return Value

A list of source tensors.

## See Also

### Inspecting Graphs

func resultTensors(for: MLCLayer) -> [MLCTensor]

Gets the result tensors for a layer in the training graph.

Deprecated

var device: MLCDevice?

The device you’ll use for compiling and executing a graph.

Deprecated

var layers: [MLCLayer]

An array that contains the layers in the graph.

Deprecated

var summarizedDOTDescription: String

A DOT representation of the graph.

Deprecated

