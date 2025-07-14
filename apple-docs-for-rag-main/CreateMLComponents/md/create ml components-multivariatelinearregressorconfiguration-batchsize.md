

- Create ML Components
- MultivariateLinearRegressorConfiguration
-  batchSize 

Instance Property

# batchSize

The number of examples in each training batch.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var batchSize: Int
```

## Discussion

Note

This parameter is only used by the `fitted` method.

## See Also

### Getting the properties

var maximumIterationCount: Int

The maximum number of allowed passes through the data.

var earlyStoppingTolerance: Float

The early-stopping tolerance.

var earlyStoppingIterationCount: Int

The number of iterations to use when evaluating whether to stop early.

var learningRate: Float

The optimizer learning rate.

var randomSeed: Int?

A seed to generate reproducible results from random operations.

