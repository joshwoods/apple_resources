

- Create ML
- MLDecisionTreeRegressor
-  MLDecisionTreeRegressor.ModelParameters 

Structure

# MLDecisionTreeRegressor.ModelParameters

Parameters that affect the process of training a model.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
struct ModelParameters
```

## Topics

### Creating parameters

init(validation: MLDecisionTreeRegressor.ModelParameters.ValidationData, maxDepth: Int, minLossReduction: Double, minChildWeight: Double, randomSeed: Int)

init(validationData: MLDataTable?, maxDepth: Int, minLossReduction: Double, minChildWeight: Double, randomSeed: Int)

Creates a new set of parameters.

Deprecated

enum ValidationData

Values for specifying validation data.

### Accessing parameters

var maxDepth: Int

var minChildWeight: Double

var minLossReduction: Double

var randomSeed: Int

var validationData: MLDataTable?

Validation data represented as a `MLDataTable`.

Deprecated

var validation: MLDecisionTreeRegressor.ModelParameters.ValidationData

Validation data.

### Describing parameters

var description: String

A text representation of the model parameters for a decision tree regressor.

var debugDescription: String

A text representation of the model parameters for a decision tree regressor that’s suitable for output during debugging.

var playgroundDescription: Any

A text representation of the model parameters for a decision tree regressor.

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

### Creating and training a decision tree regressor

init(checkpoint: MLCheckpoint) throws

Creates a decision tree regressor from a checkpoint.

init(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLDecisionTreeRegressor.ModelParameters) throws

Creates a decision tree regressor.

static func makeTrainingSession(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLDecisionTreeRegressor.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLDecisionTreeRegressor>

Creates or restores a training session.

static func makeTrainingSession(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLDecisionTreeRegressor.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLDecisionTreeRegressor>

Creates or restores a training session.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLDecisionTreeRegressor>

Restores an existing training session.

static func resume(MLTrainingSession&lt;MLDecisionTreeRegressor>) throws -> MLJob&lt;MLDecisionTreeRegressor>

Resumes a training session from the last checkpoint if available.

static func train(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLDecisionTreeRegressor.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLDecisionTreeRegressor>

Trains a decision tree regressor.

static func train(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLDecisionTreeRegressor.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLDecisionTreeRegressor>

Trains a decision tree regressor.

init(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLDecisionTreeRegressor.ModelParameters) throws

Creates a Decision Tree Regressor from the feature columns in the training data to predict the values in the target column.

Deprecated

let modelParameters: MLDecisionTreeRegressor.ModelParameters

The underlying parameters used when training the model.

var targetColumn: String

The name of the column you selected at initialization to define which feature the regressor predicts.

var featureColumns: [String]

The names of the columns you selected at initialization to train the regressor.

