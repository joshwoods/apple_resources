

- Create ML Components
- MultivariateLinearRegressorConfiguration
-  maximumIterationCount 

Instance Property

# maximumIterationCount

The maximum number of allowed passes through the data.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var maximumIterationCount: Int
```

## Discussion

More passes over the data can result in a more accurately trained model. Consider increasing this if the training accuracy is low. Defaults to 25.

Note

This parameter is only used by the `fitted` method. When using the `update` method it’s up to you to decide when to stop.

## See Also

### Getting the properties

var batchSize: Int

The number of examples in each training batch.

var earlyStoppingTolerance: Float

The early-stopping tolerance.

var earlyStoppingIterationCount: Int

The number of iterations to use when evaluating whether to stop early.

var learningRate: Float

The optimizer learning rate.

var randomSeed: Int?

A seed to generate reproducible results from random operations.

