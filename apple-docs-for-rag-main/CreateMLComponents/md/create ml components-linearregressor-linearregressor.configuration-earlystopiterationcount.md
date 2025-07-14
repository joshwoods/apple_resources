

- Create ML Components
- LinearRegressor
- LinearRegressor.Configuration
-  earlyStopIterationCount 

Instance Property

# earlyStopIterationCount

The number of iterations to use when evaluating whether to stop early.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
var earlyStopIterationCount: Int
```

## Discussion

The `fitted` method will stop if no significant progress is made for this many iterations. Significant progress happens when the validation error decreases by at least `convergenceThreshold`.

Note

Early stopping only happens when using the `fitted` method with validation data.

## See Also

### Getting the properties

var convergenceThreshold: Double

The convergence threshold.

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

var stepSize: Double

The starting step size to use for the solver.

