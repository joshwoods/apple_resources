

- Create ML Components
- FullyConnectedNetworkConfiguration
-  batchSize 

Instance Property

# batchSize

The number of examples to use per mini-batch.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
var batchSize: Int
```

## Discussion

A larger batch size will speed up computation when training, as long as the batch fits in memory.

Note

This parameter is only used by the `fitted` method. When using the `update` method it’s up to you to do batching.

## See Also

### Getting the properties

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

var maximumIterations: Int

The maximum number of iterations.

var randomSeed: Int

A seed to generate reproducible results from random operations such as column and row subsampling.

