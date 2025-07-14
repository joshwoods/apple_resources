

- Create ML
- MLTextClassifier
- MLTextClassifier.ModelParameters
-  validation 

Instance Property

# validation

The validation dataset.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
var validation: MLTextClassifier.ModelParameters.ValidationData { get set }
```

## Discussion

The default value is MLTextClassifier.ModelParameters.ValidationData.split(strategy:) with the MLSplitStrategy.automatic split strategy\`\`, which automatically generates the validation dataset by partitioning up to 10% of the training dataset.

## See Also

### Accessing parameters

var algorithm: MLTextClassifier.ModelAlgorithmType

The parameter’s algorithm setting.

var language: NLLanguage?

The parameter’s language setting.

var maxIterations: Int?

The maximum number of training iterations.

