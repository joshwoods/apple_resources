

- Create ML
- MLWordTagger
-  init(trainingData:parameters:) 

Initializer

# init(trainingData:parameters:)

Creates a word tagger.

macOS 10.15+

``` source
init(
    trainingData: [(tokens: [MLWordTagger.Token], labels: [String])],
    parameters: MLWordTagger.ModelParameters = ModelParameters(validation: .split(strategy: .automatic))
) throws
```

## Parameters 

`trainingData`  

An array of tuples containing the tokens and their labels.

`parameters`  

The model parameters.

## See Also

### Creating and training a word tagger

init(trainingData: MLDataTable, tokenColumn: String, labelColumn: String, parameters: MLWordTagger.ModelParameters) throws

Creates a word tagger.

Deprecated

init(trainingData: DataFrame, tokenColumn: String, labelColumn: String, parameters: MLWordTagger.ModelParameters) throws

Creates a word tagger.

typealias Token

The token type of a word tagger, which is a string.

struct ModelParameters

Parameters that specify model training parameters and validation data.

let modelParameters: MLWordTagger.ModelParameters

The configuration parameters that the word tagger used for training during initialization.

