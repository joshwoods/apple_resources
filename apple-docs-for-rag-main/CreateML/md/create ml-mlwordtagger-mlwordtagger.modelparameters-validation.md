

- Create ML
- MLWordTagger
- MLWordTagger.ModelParameters
-  validation 

Instance Property

# validation

The validation dataset.

macOS 10.15+

``` source
var validation: MLWordTagger.ModelParameters.ValidationData { get set }
```

## Discussion

The default value is an MLWordTagger.ModelParameters.ValidationData.split(strategy:) instance with the MLSplitStrategy.automatic split strategy\`\`, which automatically generates the validation dataset by partitioning up to 10% of the training dataset.

## See Also

### Accessing parameters

var algorithm: MLWordTagger.ModelAlgorithmType

The algorithm type.

var language: NLLanguage?

The language setting.

var maxIterations: Int?

The maximum training iterations.

