

- Create ML
-  MLLinearRegressor 

Structure

# MLLinearRegressor

A regressor that estimates the target as a linear function of the features.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
struct MLLinearRegressor
```

## Topics

### Creating and Training a Linear Regressor

init(checkpoint: MLCheckpoint) throws

Creates a linear regressor from a checkpoint.

init(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLLinearRegressor.ModelParameters) throws

Creates a linear regressor.

static func makeTrainingSession(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLLinearRegressor.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLLinearRegressor>

Creates or restores a training session.

static func makeTrainingSession(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLLinearRegressor.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLLinearRegressor>

Creates or restores a training session.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLLinearRegressor>

Restores an existing training session.

static func resume(MLTrainingSession&lt;MLLinearRegressor>) throws -> MLJob&lt;MLLinearRegressor>

Resumes a training session from the last checkpoint if available.

static func train(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLLinearRegressor.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLLinearRegressor>

Trains a linear regressor.

static func train(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLLinearRegressor.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLLinearRegressor>

Trains a linear regressor.

init(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLLinearRegressor.ModelParameters) throws

Creates a Linear Regressor from the feature columns in the training data to predict the values in the target column.

Deprecated

struct ModelParameters

Parameters that affect the process of training a model.

let modelParameters: MLLinearRegressor.ModelParameters

The underlying parameters used when training the model.

var targetColumn: String

The name of the column you selected at initialization to define which feature the regressor predicts.

var featureColumns: [String]

The names of the columns you selected at initialization to train the regressor.

### Assessing Model Accuracy

var trainingMetrics: MLRegressorMetrics

Measurements of the regressor’s performance on the training data set.

var validationMetrics: MLRegressorMetrics

Measurements of the regressor’s performance on the validation data set.

### Evaluating a Linear Regressor

func evaluation(on: DataFrame) -> MLRegressorMetrics

Evaluates the classifier on the provided labeled data.

func evaluation(on: MLDataTable) -> MLRegressorMetrics

Evaluates the classifier on the provided labeled data.

Deprecated

### Testing a Linear Regressor

func predictions(from: DataFrame) throws -> AnyColumn

Predicts a column of labels for the given testing data.

func predictions(from: MLDataTable) throws -> MLUntypedColumn

Predicts the target value from the provided data.

Deprecated

### Saving a Linear Regressor

func write(to: URL, metadata: MLModelMetadata?) throws

Exports a Core ML model file for use in your app.

func write(toFile: String, metadata: MLModelMetadata?) throws

Exports a Core ML model file for use in your app.

### Describing a Linear Regressor

var model: MLModel

The Core ML model.

var description: String

A text representation of the linear regressor.

var debugDescription: String

A text representation of the linear regressor that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the linear regressor shown in a playground.

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
- Sendable

## See Also

### Supporting regressor types

struct MLDecisionTreeRegressor

A regressor that estimates the target by learning rules to split the data.

struct MLRandomForestRegressor

A regressor based on a collection of decision trees trained on subsets of the data.

struct MLBoostedTreeRegressor

A regressor based on a collection of decision trees combined with gradient boosting.

