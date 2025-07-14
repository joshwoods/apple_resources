

- Create ML Components
- FullyConnectedNetworkConfiguration
-  earlyStopIterationCount 

Instance Property

# earlyStopIterationCount

The number of iterations to use when evaluating whether to stop early.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
var earlyStopIterationCount: Int
```

## Discussion

The `fitted` method will stop if no significant progress is made for this many iterations. Significant progress happens when the validation loss decreases by at least `earlyStoppingTolerance`.

Defaults to 10.

Note

Early stopping only happens when using the `fitted` method with validation data.

## See Also

### Getting the properties

var batchSize: Int

The number of examples to use per mini-batch.

var dropoutProbability: Float

The dropout probability.

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

