

- Create ML Components
- BoostedTreeConfiguration
-  stepSize 

Instance Property

# stepSize

The step size shrinking.

iOS 16.0–17.0DeprecatediPadOS 16.0–17.0DeprecatedMac Catalyst 16.0–17.0DeprecatedmacOS 13.0–14.0DeprecatedtvOS 16.0–17.0DeprecatedvisionOS 1.0+watchOS 11.0+

``` source
var stepSize: Double { get set }
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

var randomSeed: Int

A seed to generate reproducible results from random operations such as column and row subsampling.

var rowSubsample: Double

Subsample ratio of the training set in each iteration of tree construction.

