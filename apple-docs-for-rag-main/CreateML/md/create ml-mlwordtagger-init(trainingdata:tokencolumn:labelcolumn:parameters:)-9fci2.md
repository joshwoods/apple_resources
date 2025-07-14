

- Create ML
- MLWordTagger
-  init(trainingData:tokenColumn:labelColumn:parameters:) 

Initializer

# init(trainingData:tokenColumn:labelColumn:parameters:)

Creates a word tagger.

macOS 13.0+

``` source
init(
    trainingData: DataFrame,
    tokenColumn: String,
    labelColumn: String,
    parameters: MLWordTagger.ModelParameters = ModelParameters(validation: .split(strategy: .automatic))
) throws
```

## Parameters 

`trainingData`  

A data frame specifying training data.

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

init(trainingData: MLDataTable, tokenColumn: String, labelColumn: String, parameters: MLWordTagger.ModelParameters) throws

Creates a word tagger.

Deprecated

typealias Token

The token type of a word tagger, which is a string.

struct ModelParameters

Parameters that specify model training parameters and validation data.

let modelParameters: MLWordTagger.ModelParameters

The configuration parameters that the word tagger used for training during initialization.

