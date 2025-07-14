

- ML Compute
- MLCTrainingGraph
-  init(graphObjects:lossLayer:optimizer:) Deprecated

Initializer

# init(graphObjects:lossLayer:optimizer:)

Creates a training graph with the layers from the graph objects, loss layer, and optimizer you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init(
    graphObjects: [MLCGraph],
    lossLayer: MLCLayer?,
    optimizer: MLCOptimizer?
)
```

## Parameters 

`graphObjects`  

The graph objects whose layers you add to the training graph.

`lossLayer`  

The loss layer.

`optimizer`  

The optimizer.

## Discussion

You can also add a loss layer to a training graph using the node(with:sources:lossLabels:) method.

## See Also

### Creating Training Graphs

Optimizers

Create an optimizer to use with the training graph.

class MLCTensorParameter

A tensor parameter object.

Deprecated

