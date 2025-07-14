

- Create ML
- MLSupportVectorClassifier
-  MLSupportVectorClassifier.ModelParameters Deprecated

Structure

# MLSupportVectorClassifier.ModelParameters

Parameters that affect the process of training a model.

macOS 10.14–14.0Deprecated

``` source
struct ModelParameters
```

## Topics

### Creating parameters

init(validation: MLSupportVectorClassifier.ModelParameters.ValidationData, maxIterations: Int, penalty: Double, convergenceThreshold: Double, featureRescaling: Bool)

Creates a new set of parameters.

init(validationData: MLDataTable?, maxIterations: Int, penalty: Double, convergenceThreshold: Double, featureRescaling: Bool)

Creates a new set of parameters.

enum ValidationData

Values for specifying validation data.

### Accessing parameters

var convergenceThreshold: Double

var featureRescaling: Bool

var maxIterations: Int

var penalty: Double

var validationData: MLDataTable?

Validation data represented as a `MLDataTable`.

var validation: MLSupportVectorClassifier.ModelParameters.ValidationData

Validation data.

### Describing parameters

var description: String

A text representation of the model parameters for a support vector classifier.

var debugDescription: String

A text representation of the model parameters for a support vector classifier that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the model parameters for a support vector classifier shown in a playground.

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

### Creating and training a support vector classifier

init(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLSupportVectorClassifier.ModelParameters) throws

Creates a support vector classifier.

Deprecated

init(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLSupportVectorClassifier.ModelParameters) throws

Creates a Support Vector Classifier from the feature columns in the training data to predict the categories in the target column.

Deprecated

let modelParameters: MLSupportVectorClassifier.ModelParameters

The underlying parameters used when training the model.

Deprecated

var targetColumn: String

The name of the column you selected at initialization to define which categories the classifier predicts.

Deprecated

var featureColumns: [String]

The names of the columns you selected at initialization to train the classifier.

Deprecated

