

- Create ML
- MLWordTagger
- MLWordTagger.ModelParameters
-  validationData Deprecated

Instance Property

# validationData

The word tagger’s validation dataset as a data table.

macOS 10.14–10.15Deprecated

``` source
var validationData: MLDataTable? { get set }
```

Deprecated

Use the validation property instead.

## See Also

### Deprecated

init(validationData: MLDataTable?, algorithm: MLWordTagger.ModelAlgorithmType, language: NLLanguage?, tokenColumnValidationData: String?, labelColumnValidationData: String?)

Creates model parameters.

Deprecated

init(validationData: [(tokens: [MLWordTagger.Token], labels: [String])], algorithm: MLWordTagger.ModelAlgorithmType, language: NLLanguage?)

Creates model parameters.

Deprecated

var tokenColumnValidationData: String?

The name of the column containing the tokens in the validation data table.

Deprecated

var labelColumnValidationData: String?

The name of the column containing the token labels in the validation data table.

Deprecated

