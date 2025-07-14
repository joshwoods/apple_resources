

- Create ML
- MLWordTagger
-  modelParameters 

Instance Property

# modelParameters

The configuration parameters that the word tagger used for training during initialization.

macOS 10.14+

``` source
let modelParameters: MLWordTagger.ModelParameters
```

## See Also

### Creating and training a word tagger

init(trainingData: [(tokens: [MLWordTagger.Token], labels: [String])], parameters: MLWordTagger.ModelParameters) throws

Creates a word tagger.

init(trainingData: MLDataTable, tokenColumn: String, labelColumn: String, parameters: MLWordTagger.ModelParameters) throws

Creates a word tagger.

Deprecated

init(trainingData: DataFrame, tokenColumn: String, labelColumn: String, parameters: MLWordTagger.ModelParameters) throws

Creates a word tagger.

typealias Token

The token type of a word tagger, which is a string.

struct ModelParameters

Parameters that specify model training parameters and validation data.

