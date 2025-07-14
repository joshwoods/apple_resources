

- Create ML Components
- LogisticRegressionClassifier
- LogisticRegressionClassifier.Configuration
-  scaleFeatures 

Instance Property

# scaleFeatures

A Boolean value indicating whether to scale the input features.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
var scaleFeatures: Bool
```

## Discussion

Scaling the features reduces numerical errors.

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

var stepSize: Double

The starting step size to use for the solver.

