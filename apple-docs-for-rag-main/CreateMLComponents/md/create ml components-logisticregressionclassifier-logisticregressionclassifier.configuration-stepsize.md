

- Create ML Components
- LogisticRegressionClassifier
- LogisticRegressionClassifier.Configuration
-  stepSize 

Instance Property

# stepSize

The starting step size to use for the solver.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
var stepSize: Double
```

## Discussion

Defaults to 1.0. If the first iteration takes a considerable amount of time, reducing this parameter may speed up model training.

## See Also

### Getting the properties

var convergenceThreshold: Double

The convergence threshold.

var earlyStopIterationCount: Int

The number of iterations to use when evaluating whether to stop early.

var l1Penalty: Double

Weight of the L1 regularization term.

var l2Penalty: Double

Weight of the L2 regularization term.

var maximumIterations: Int

The maximum number of allowed passes through the data.

var optimizationStrategy: OptimizationStrategy

The optimization strategy.

var scaleFeatures: Bool

A Boolean value indicating whether to scale the input features.

