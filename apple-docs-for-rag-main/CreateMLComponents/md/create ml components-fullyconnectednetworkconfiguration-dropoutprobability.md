

- Create ML Components
- FullyConnectedNetworkConfiguration
-  dropoutProbability 

Instance Property

# dropoutProbability

The dropout probability.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
var dropoutProbability: Float
```

## Discussion

Dropout layers are placed after fully-connected layers to help prevent over-fitting.

Defaults to 0.2.

## See Also

### Getting the properties

var batchSize: Int

The number of examples to use per mini-batch.

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

