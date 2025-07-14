

- Create ML Components
- FullyConnectedNetworkConfiguration
-  learningRate 

Instance Property

# learningRate

The learning rate.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
var learningRate: Float
```

## Discussion

The learning rate controls how much the model changes when presented with new data. A high learning rate may overshoot when close to a solution, while a low learning rate my take too long to train a good model.

Defaults to 0.001.

## See Also

### Getting the properties

var batchSize: Int

The number of examples to use per mini-batch.

var dropoutProbability: Float

The dropout probability.

var earlyStopIterationCount: Int

The number of iterations to use when evaluating whether to stop early.

var earlyStoppingTolerance: Double

The early-stopping tolerance.

var hiddenUnitCounts: [Int]

The number of neurons in each hidden layer.

var maximumIterations: Int

The maximum number of iterations.

var randomSeed: Int

A seed to generate reproducible results from random operations such as column and row subsampling.

