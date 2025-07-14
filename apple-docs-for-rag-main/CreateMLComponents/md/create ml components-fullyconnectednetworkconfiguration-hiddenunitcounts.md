

- Create ML Components
- FullyConnectedNetworkConfiguration
-  hiddenUnitCounts 

Instance Property

# hiddenUnitCounts

The number of neurons in each hidden layer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
var hiddenUnitCounts: [Int]
```

## Discussion

Defaults to a single hidden layer with 100 neurons.

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

var learningRate: Float

The learning rate.

var maximumIterations: Int

The maximum number of iterations.

var randomSeed: Int

A seed to generate reproducible results from random operations such as column and row subsampling.

