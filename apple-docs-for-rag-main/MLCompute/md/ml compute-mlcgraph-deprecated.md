

- ML Compute
-  MLCGraph Deprecated

Class

# MLCGraph

A graph of layers you use to build a training or inference graph.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCGraph
```

## Topics

### Adding Layers to Graphs

func node(with: MLCLayer, source: MLCTensor) -> MLCTensor?

Adds the layer and source tensor that you specify to the graph.

func node(with: MLCLayer, sources: [MLCTensor]) -> MLCTensor?

Adds the layer and source tensors that you specify to the graph.

func node(with: MLCLayer, sources: [MLCTensor], disableUpdate: Bool) -> MLCTensor?

Adds the layer, source tensors, and option to disable optimizer updates that you specify to the graph.

func node(with: MLCLayer, sources: [MLCTensor], lossLabels: [MLCTensor]) -> MLCTensor?

Adds the layer, sources, and loss labels tensors that you specify to the graph.

### Adding New Layers to Graphs

func split(source: MLCTensor, splitCount: Int, dimension: Int) -> [MLCTensor]?

Adds a new split layer to the graph using the source tensor, number of splits, and dimension to split the source tensor that you specify.

func split(source: MLCTensor, splitSectionLengths: [Int], dimension: Int) -> [MLCTensor]?

Adds a new split layer to the graph using the source tensor, lengths of each split section, and dimension to split the source tensor that you specify.

func concatenate(sources: [MLCTensor], dimension: Int) -> MLCTensor?

Adds a new concatenation layer to the graph using the source tensors and concatenation dimension you specify.

func reshape(shape: [Int], source: MLCTensor) -> MLCTensor?

Adds a new reshape layer to the graph using the shape and source tensor you specify.

func gather(withDimension: Int, source: MLCTensor, indices: MLCTensor) -> MLCTensor?

Adds a gather layer to the graph using the source tensor, dimension along which to index, and the indices you specify.

func scatter(withDimension: Int, source: MLCTensor, indices: MLCTensor, copyFrom: MLCTensor, reductionType: MLCReductionType) -> MLCTensor?

Adds a scatter layer to the graph.

func transpose(dimensions: [Int], source: MLCTensor) -> MLCTensor?

Adds a new transpose layer to the graph using the dimensions and source tensor you specify.

### Associating Data with Input Tensors

func bindAndWriteData([String : MLCTensorData], forInputs: [String : MLCTensor], to: MLCDevice, batchSize: Int, synchronous: Bool) -> Bool

Associates the given data with the input tensors, and if the device is a GPU, also copies the data to the device memory.

func bindAndWriteData([String : MLCTensorData], forInputs: [String : MLCTensor], to: MLCDevice, synchronous: Bool) -> Bool

Associates the given data with the input tensors, and if the device is a GPU, also copies the data to the device memory.

### Inspecting Graphs

func sourceTensors(for: MLCLayer) -> [MLCTensor]

Gets the source tensors for a layer in the training graph.

func resultTensors(for: MLCLayer) -> [MLCTensor]

Gets the result tensors for a layer in the training graph.

var device: MLCDevice?

The device you’ll use for compiling and executing a graph.

var layers: [MLCLayer]

An array that contains the layers in the graph.

var summarizedDOTDescription: String

A DOT representation of the graph.

## Relationships

### Inherits From

- NSObject

### Inherited By

- MLCInferenceGraph
- MLCTrainingGraph

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Graphs

class MLCTrainingGraph

A training graph that you create from one or more graph objects plus additional layers you add directly to the training graph.

Deprecated

class MLCInferenceGraph

An inference graph created from one or more MLCGraph instances plus additional layers added directly to the inference graph.

Deprecated

