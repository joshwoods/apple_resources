

- Create ML Components
- MultivariateLinearRegressorConfiguration
-  learningRate 

Instance Property

# learningRate

The optimizer learning rate.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var learningRate: Float
```

## Discussion

Defaults to 0.005.

## See Also

### Getting the properties

var batchSize: Int

The number of examples in each training batch.

var maximumIterationCount: Int

The maximum number of allowed passes through the data.

var earlyStoppingTolerance: Float

The early-stopping tolerance.

var earlyStoppingIterationCount: Int

The number of iterations to use when evaluating whether to stop early.

var randomSeed: Int?

A seed to generate reproducible results from random operations.

