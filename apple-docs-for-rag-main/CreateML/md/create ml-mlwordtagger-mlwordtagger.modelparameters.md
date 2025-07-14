

- Create ML
- MLWordTagger
-  MLWordTagger.ModelParameters 

Structure

# MLWordTagger.ModelParameters

Parameters that specify model training parameters and validation data.

macOS 10.14+

``` source
struct ModelParameters
```

## Topics

### Creating parameters

init(validation: MLWordTagger.ModelParameters.ValidationData, algorithm: MLWordTagger.ModelAlgorithmType, language: NLLanguage?)

Creates model parameters.

enum ModelAlgorithmType

The algorithm type.

enum ValidationData

The validation data.

### Accessing parameters

var algorithm: MLWordTagger.ModelAlgorithmType

The algorithm type.

var language: NLLanguage?

The language setting.

var validation: MLWordTagger.ModelParameters.ValidationData

The validation dataset.

var maxIterations: Int?

The maximum training iterations.

### Describing parameters

var description: String

A text representation of the model parameters.

var debugDescription: String

A text representation of the model parameters that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the model parameters in a playground.

### Deprecated

init(validationData: MLDataTable?, algorithm: MLWordTagger.ModelAlgorithmType, language: NLLanguage?, tokenColumnValidationData: String?, labelColumnValidationData: String?)

Creates model parameters.

Deprecated

init(validationData: [(tokens: [MLWordTagger.Token], labels: [String])], algorithm: MLWordTagger.ModelAlgorithmType, language: NLLanguage?)

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

### Default Implementations

CustomDebugStringConvertible Implementations

CustomPlaygroundDisplayConvertible Implementations

CustomStringConvertible Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomPlaygroundDisplayConvertible
- CustomStringConvertible

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

let modelParameters: MLWordTagger.ModelParameters

The configuration parameters that the word tagger used for training during initialization.

