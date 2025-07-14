

- Create ML
- MLTextClassifier
-  MLTextClassifier.ModelParameters 

Structure

# MLTextClassifier.ModelParameters

Parameters that specify model training parameters and validation data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
struct ModelParameters
```

## Topics

### Creating parameters

init(validation: MLTextClassifier.ModelParameters.ValidationData, algorithm: MLTextClassifier.ModelAlgorithmType, language: NLLanguage?)

Creates model parameters for a text classifier with the specified validation data, algorithm, and language.

struct NLLanguage

The languages that the Natural Language framework supports.

enum ModelAlgorithmType

The type of algorithm that a text classifier uses.

enum ValidationData

The validation data that a text classifier uses.

### Accessing parameters

var algorithm: MLTextClassifier.ModelAlgorithmType

The parameter’s algorithm setting.

var language: NLLanguage?

The parameter’s language setting.

var validation: MLTextClassifier.ModelParameters.ValidationData

The validation dataset.

var maxIterations: Int?

The maximum number of training iterations.

### Describing parameters

var description: String

A text representation of the model parameters.

var debugDescription: String

A text representation of the model parameters that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the model parameters in a playground.

### Deprecated

init(validationData: [String : [String]], algorithm: MLTextClassifier.ModelAlgorithmType, language: NLLanguage?)

Creates parameters for a text classifier with validation data in a dictionary.

Deprecated

init(validationData: MLDataTable?, algorithm: MLTextClassifier.ModelAlgorithmType, language: NLLanguage?, textColumnValidationData: String?, labelColumnValidationData: String?)

Creates parameters for a text classifier with validation data in a data table.

Deprecated

init(validationData: MLTextClassifier.DataSource, algorithm: MLTextClassifier.ModelAlgorithmType, language: NLLanguage?)

Creates parameters for a text classifier with validation data in a set of labeled directories.

Deprecated

var validationData: MLDataTable?

The validation data.

Deprecated

var textColumnValidationData: String?

The name of the text column in the validation data table.

Deprecated

var labelColumnValidationData: String?

The name of the label column in the validation data table.

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

### Creating and training a text classifier

init(trainingData: [String : [String]], parameters: MLTextClassifier.ModelParameters) throws

Creates a text classifier.

init(trainingData: DataFrame, textColumn: String, labelColumn: String, parameters: MLTextClassifier.ModelParameters) throws

Creates a text classifier.

init(trainingData: MLTextClassifier.DataSource, parameters: MLTextClassifier.ModelParameters) throws

Creates a text classifier.

enum DataSource

A data source for a text classifier.

let modelParameters: MLTextClassifier.ModelParameters

The configuration parameters that the text classifier used for training during initialization.

init(trainingData: MLDataTable, textColumn: String, labelColumn: String, parameters: MLTextClassifier.ModelParameters) throws

Creates a text classifier.

Deprecated

