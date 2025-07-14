

- Create ML
- MLWordTagger
-  init(trainingData:tokenColumn:labelColumn:parameters:) Deprecated

Initializer

# init(trainingData:tokenColumn:labelColumn:parameters:)

Creates a word tagger.

macOS 10.14–13.0Deprecated

``` source
init(
    trainingData: MLDataTable,
    tokenColumn: String,
    labelColumn: String,
    parameters: MLWordTagger.ModelParameters = ModelParameters(validationData: nil)
) throws
```

Deprecated

Use DataFrame instead of MLDataTable when initializing.

## Parameters 

`trainingData`  

A table specifying training data.

`tokenColumn`  

The name of the token column in the training data frame.

`labelColumn`  

The name of the label column in the training data frame.

`parameters`  

The model parameters.

## See Also

### Creating and training a word tagger

init(trainingData: [(tokens: [MLWordTagger.Token], labels: [String])], parameters: MLWordTagger.ModelParameters) throws

Creates a word tagger.

init(trainingData: DataFrame, tokenColumn: String, labelColumn: String, parameters: MLWordTagger.ModelParameters) throws

Creates a word tagger.

typealias Token

The token type of a word tagger, which is a string.

struct ModelParameters

Parameters that specify model training parameters and validation data.

let modelParameters: MLWordTagger.ModelParameters

The configuration parameters that the word tagger used for training during initialization.

