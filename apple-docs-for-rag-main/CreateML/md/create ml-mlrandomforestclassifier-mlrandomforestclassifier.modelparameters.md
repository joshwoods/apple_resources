

- Create ML
- MLRandomForestClassifier
-  MLRandomForestClassifier.ModelParameters 

Structure

# MLRandomForestClassifier.ModelParameters

Parameters that affect the process of training a model.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
struct ModelParameters
```

## Topics

### Creating parameters

init(validation: MLRandomForestClassifier.ModelParameters.ValidationData, maxDepth: Int, maxIterations: Int, minLossReduction: Double, minChildWeight: Double, randomSeed: Int, rowSubsample: Double, columnSubsample: Double)

init(validationData: MLDataTable?, maxDepth: Int, maxIterations: Int, minLossReduction: Double, minChildWeight: Double, randomSeed: Int, rowSubsample: Double, columnSubsample: Double)

Creates a new set of parameters.

Deprecated

enum ValidationData

Values for specifying validation data.

### Accessing parameters

var columnSubsample: Double

Must be in the range (0, 1).

var maxDepth: Int

var maxIterations: Int

var minChildWeight: Double

var minLossReduction: Double

var randomSeed: Int

var rowSubsample: Double

Must be in the range (0, 1).

var validationData: MLDataTable?

Validation data represented as a `MLDataTable`.

Deprecated

var validation: MLRandomForestClassifier.ModelParameters.ValidationData

Validation data.

### Describing parameters

var description: String

A text representation of the model parameters for a random forest classifier.

var debugDescription: String

A text representation of the model parameters for a random forest classifier that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the model parameters for a random forest classifier shown in a playground.

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

### Creating and training a random forest classifier

init(checkpoint: MLCheckpoint) throws

Creates a random forest classifier classifier from a checkpoint.

init(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLRandomForestClassifier.ModelParameters) throws

Creates a random forest classifier.

init(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLRandomForestClassifier.ModelParameters) throws

Creates a Random Forest Classifier from the feature columns in the training data to predict the categories in the target column.

Deprecated

let modelParameters: MLRandomForestClassifier.ModelParameters

The underlying parameters used when training the model.

var targetColumn: String

The name of the column you selected at initialization to define which categories the classifier predicts.

var featureColumns: [String]

The names of the columns you selected at initialization to train the classifier.

