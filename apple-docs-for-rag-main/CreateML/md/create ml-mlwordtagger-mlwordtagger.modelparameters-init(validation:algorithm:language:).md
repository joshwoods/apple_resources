

- Create ML
- MLWordTagger
- MLWordTagger.ModelParameters
-  init(validation:algorithm:language:) 

Initializer

# init(validation:algorithm:language:)

Creates model parameters.

macOS 10.15+

``` source
init(
    validation: MLWordTagger.ModelParameters.ValidationData = .split(strategy: .automatic),
    algorithm: MLWordTagger.ModelAlgorithmType = .crf(revision: 1),
    language: NLLanguage? = nil
)
```

## Parameters 

`validation`  

The validation data source.

`algorithm`  

The algorithm type.

`language`  

The language of the text to tag.

## See Also

### Creating parameters

enum ModelAlgorithmType

The algorithm type.

enum ValidationData

The validation data.

