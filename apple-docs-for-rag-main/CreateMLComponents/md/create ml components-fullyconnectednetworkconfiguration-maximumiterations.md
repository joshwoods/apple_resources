

- Create ML Components
- FullyConnectedNetworkConfiguration
-  maximumIterations 

Instance Property

# maximumIterations

The maximum number of iterations.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
var maximumIterations: Int
```

## Discussion

More iterations will produce better models as long as there is no over-fitting. Over-fitting happens when the dropout probability is too low or there is not enough training data.

Note

This parameter is only used by the `fitted` method. When using the `update` method it’s up to you to decide when to stop.

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

var learningRate: Float

The learning rate.

var randomSeed: Int

A seed to generate reproducible results from random operations such as column and row subsampling.

