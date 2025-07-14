

- Create ML
- MLLogisticRegressionClassifier
- MLLogisticRegressionClassifier.ModelParameters
-  validation 

Instance Property

# validation

Validation data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+tvOS 16.0+visionOS 1.0+

``` source
var validation: MLLogisticRegressionClassifier.ModelParameters.ValidationData { get set }
```

## Discussion

The default is `.split(strategy: .automatic)`, which automatically generates the validation dataset from 0% to 10% of the training dataset.

## See Also

### Accessing parameters

var convergenceThreshold: Double

var featureRescaling: Bool

var l1Penalty: Double

var l2Penalty: Double

var maxIterations: Int

var stepSize: Double

var validationData: MLDataTable?

Validation data represented as a `MLDataTable`.

Deprecated

