

- Create ML Components
- OptimizationStrategy
-  OptimizationStrategy.nonSmooth 

Case

# OptimizationStrategy.nonSmooth

An optimization strategy that can handle non-smooth problems.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
case nonSmooth
```

## Discussion

Select this strategy when using L1 regularization. Using L1 regularization causes the optimization problem to be non-smooth. Other optimization strategies rely on the optimization problem being smooth and will likely fail to converge when using L1 regularization.

## See Also

### Optimization strategies

case automatic

Chooses the best optimization strategy based on the problem size and configuration.

case fast

An optimization strategy that minimizes computation time.

case lowMemory

An optimization strategy that minimizes memory use.

