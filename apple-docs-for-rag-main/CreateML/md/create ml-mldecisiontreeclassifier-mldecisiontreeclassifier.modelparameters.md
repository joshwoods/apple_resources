

- Create ML
- MLDecisionTreeClassifier
-  MLDecisionTreeClassifier.ModelParameters 

Structure

# MLDecisionTreeClassifier.ModelParameters

Parameters that affect the process of training a model.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
struct ModelParameters
```

## Topics

### Creating parameters

init(validation: MLDecisionTreeClassifier.ModelParameters.ValidationData, maxDepth: Int, minLossReduction: Double, minChildWeight: Double, randomSeed: Int)

init(validationData: MLDataTable?, maxDepth: Int, minLossReduction: Double, minChildWeight: Double, randomSeed: Int)

Creates a new set of parameters.

Deprecated

enum ValidationData

Values for specifying validation data.

### Accessing parameters

var validationData: MLDataTable?

The data used for the validation set to inform the model training process.

Deprecated

var maxDepth: Int

The maximum depth of the tree. Must be greater than 0.

var minLossReduction: Double

The minimum amount that the loss needs to be reduced to create a new split.

var minChildWeight: Double

The minimum weight of each leaf node.

var randomSeed: Int

The seed value for random operations during tree building process.

var validation: MLDecisionTreeClassifier.ModelParameters.ValidationData

Validation data.

### Describing parameters

var description: String

A text representation of the model parameters for a decision tree classifier.

var debugDescription: String

A text representation of the model parameters for a decision tree classifier that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the model parameters for a decision tree classifier shown in a playground.

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

### Creating and training a decision tree classifier

init(checkpoint: MLCheckpoint) throws

Creates a decision tree classifier classifier from a checkpoint.

init(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLDecisionTreeClassifier.ModelParameters) throws

Creates a decision tree classifier.

static func makeTrainingSession(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLDecisionTreeClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLDecisionTreeClassifier>

Creates or restores a training session.

static func makeTrainingSession(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLDecisionTreeClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLDecisionTreeClassifier>

Creates or restores a training session.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLDecisionTreeClassifier>

Restores an existing training session.

static func resume(MLTrainingSession&lt;MLDecisionTreeClassifier>) throws -> MLJob&lt;MLDecisionTreeClassifier>

Resumes a training session from the last checkpoint if available.

static func train(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLDecisionTreeClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLDecisionTreeClassifier>

Trains a decision tree classifier.

static func train(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLDecisionTreeClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLDecisionTreeClassifier>

Trains a decision tree classifier.

init(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLDecisionTreeClassifier.ModelParameters) throws

Creates a Decision Tree Classifier from the feature columns in the training data to predict the categories in the target column.

Deprecated

let modelParameters: MLDecisionTreeClassifier.ModelParameters

The underlying parameters used when training the model.

var targetColumn: String

The name of the column you selected at initialization to define which categories the classifier predicts.

var featureColumns: [String]

The names of the columns you selected at initialization to train the classifier.

