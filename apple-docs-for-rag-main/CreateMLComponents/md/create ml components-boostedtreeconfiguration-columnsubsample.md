

- Create ML Components
- BoostedTreeConfiguration
-  columnSubsample 

Instance Property

# columnSubsample

Subsample ratio of the columns in each iteration of tree construction.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
var columnSubsample: Double
```

## Discussion

Like row subsample, this can also help prevent model overfitting. Setting this to a value of 0.5 results in the model randomly sampling half of the columns to grow each tree. Must be in the range (0, 1).

## See Also

### Inspecting the configuration

var earlyStoppingIterationCount: Int?

Stops training after this number of iterations where the validation metric does not improve.

var learningRate: Double

The learning rate.

var maximumDepth: Int

Maximum tree depth.

var maximumIterations: Int

Maximum number of iterations.

var minimumChildWeight: Double

The minimum weight of each leaf node.

var minimumLossReduction: Double

Minimum loss reduction required to further split a node during the tree learning phase.

var parallelTreeCount: Int

The number of parallel trees constructed during each iteration.

var randomSeed: Int

A seed to generate reproducible results from random operations such as column and row subsampling.

var rowSubsample: Double

Subsample ratio of the training set in each iteration of tree construction.

var stepSize: Double

The step size shrinking.

