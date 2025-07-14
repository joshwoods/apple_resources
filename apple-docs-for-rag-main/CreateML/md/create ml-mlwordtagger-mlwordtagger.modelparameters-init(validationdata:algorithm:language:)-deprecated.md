

- Create ML
- MLWordTagger
- MLWordTagger.ModelParameters
-  init(validationData:algorithm:language:) Deprecated

Initializer

# init(validationData:algorithm:language:)

Creates model parameters.

macOS 10.14–10.15Deprecated

``` source
init(
    validationData: [(tokens: [MLWordTagger.Token], labels: [String])],
    algorithm: MLWordTagger.ModelAlgorithmType = .crf(revision: 1),
    language: NLLanguage? = nil
)
```

Deprecated

Use the validation property instead.

## Parameters 

`validationData`  

The validation data of token and label pairs.

`algorithm`  

The algorithm type.

`language`  

The language of the text to tag.

## See Also

### Deprecated

init(validationData: MLDataTable?, algorithm: MLWordTagger.ModelAlgorithmType, language: NLLanguage?, tokenColumnValidationData: String?, labelColumnValidationData: String?)

Creates model parameters.

Deprecated

var validationData: MLDataTable?

The word tagger’s validation dataset as a data table.

Deprecated

var tokenColumnValidationData: String?

The name of the column containing the tokens in the validation data table.

Deprecated

var labelColumnValidationData: String?

The name of the column containing the token labels in the validation data table.

Deprecated

