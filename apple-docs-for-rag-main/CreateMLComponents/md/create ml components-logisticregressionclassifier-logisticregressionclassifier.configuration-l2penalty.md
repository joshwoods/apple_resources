

- Create ML Components
- LogisticRegressionClassifier
- LogisticRegressionClassifier.Configuration
-  l2Penalty 

Instance Property

# l2Penalty

Weight of the L2 regularization term.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
var l2Penalty: Double
```

## Discussion

The larger this weight, the more the model coefficients shrink toward 0. This introduces bias into the model but decreases variance, potentially leading to better predictions. The default is 0.01.

## See Also

### Getting the properties

var convergenceThreshold: Double

The convergence threshold.

var earlyStopIterationCount: Int

The number of iterations to use when evaluating whether to stop early.

var l1Penalty: Double

Weight of the L1 regularization term.

var maximumIterations: Int

The maximum number of allowed passes through the data.

var optimizationStrategy: OptimizationStrategy

The optimization strategy.

var scaleFeatures: Bool

A Boolean value indicating whether to scale the input features.

var stepSize: Double

The starting step size to use for the solver.

