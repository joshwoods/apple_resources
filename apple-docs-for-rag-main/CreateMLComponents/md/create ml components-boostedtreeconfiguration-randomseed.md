

- Create ML Components
- BoostedTreeConfiguration
-  randomSeed 

Instance Property

# randomSeed

A seed to generate reproducible results from random operations such as column and row subsampling.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
var randomSeed: Int
```

## See Also

### Inspecting the configuration

var columnSubsample: Double

Subsample ratio of the columns in each iteration of tree construction.

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

var rowSubsample: Double

Subsample ratio of the training set in each iteration of tree construction.

var stepSize: Double

The step size shrinking.

