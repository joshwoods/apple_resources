

- ML Compute
- MLCGraph
-  device Deprecated

Instance Property

# device

The device you’ll use for compiling and executing a graph.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
var device: MLCDevice? { get }
```

## See Also

### Inspecting Graphs

func sourceTensors(for: MLCLayer) -> [MLCTensor]

Gets the source tensors for a layer in the training graph.

Deprecated

func resultTensors(for: MLCLayer) -> [MLCTensor]

Gets the result tensors for a layer in the training graph.

Deprecated

var layers: [MLCLayer]

An array that contains the layers in the graph.

Deprecated

var summarizedDOTDescription: String

A DOT representation of the graph.

Deprecated

