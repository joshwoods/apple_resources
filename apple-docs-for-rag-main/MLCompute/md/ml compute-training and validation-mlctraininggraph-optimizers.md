

- ML Compute
- Training and Validation
- MLCTrainingGraph
-  Optimizers 

API Collection

# Optimizers

Create an optimizer to use with the training graph.

## Topics

### Optimizer Types

class MLCSGDOptimizer

An optimizer that represents the stochastic gradient decent algorithm.

Deprecated

class MLCRMSPropOptimizer

An optimizer that represents the root mean square propagation algorithm.

class MLCAdamOptimizer

An optimizer that represents the adaptive moment estimation algorithm.

Deprecated

class MLCAdamWOptimizer

An optimizer that represents the Adam algorithm with weight decay.

Deprecated

class MLCOptimizer

The base class for all framework optimizers.

Deprecated

### Supporting Types

class MLCOptimizerDescriptor

A configuration object you use to create an optimizer.

Deprecated

enum MLCRegularizationType

A regularization function to use with an optimizer.

Deprecated

## See Also

### Creating Training Graphs

convenience init(graphObjects: [MLCGraph], lossLayer: MLCLayer?, optimizer: MLCOptimizer?)

Creates a training graph with the layers from the graph objects, loss layer, and optimizer you specify.

Deprecated

class MLCTensorParameter

A tensor parameter object.

Deprecated

