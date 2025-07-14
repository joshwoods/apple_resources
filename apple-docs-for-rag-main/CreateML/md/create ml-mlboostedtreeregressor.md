

- Create ML
-  MLBoostedTreeRegressor 

Structure

# MLBoostedTreeRegressor

A regressor based on a collection of decision trees combined with gradient boosting.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
struct MLBoostedTreeRegressor
```

## Topics

### Creating and training a boosted tree regressor

init(checkpoint: MLCheckpoint) throws

Creates a boosted tree regressor from a checkpoint.

init(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLBoostedTreeRegressor.ModelParameters) throws

Creates a boosted tree regressor.

static func makeTrainingSession(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLBoostedTreeRegressor.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLBoostedTreeRegressor>

Creates or restores a training session.

static func makeTrainingSession(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLBoostedTreeRegressor.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLBoostedTreeRegressor>

Creates or restores a training session.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLBoostedTreeRegressor>

Restores an existing training session.

static func resume(MLTrainingSession&lt;MLBoostedTreeRegressor>) throws -> MLJob&lt;MLBoostedTreeRegressor>

Resumes a training session from the last checkpoint if available.

static func train(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLBoostedTreeRegressor.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLBoostedTreeRegressor>

Trains a boosted tree regressor.

static func train(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLBoostedTreeRegressor.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLBoostedTreeRegressor>

Trains a boosted tree regressor.

init(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLBoostedTreeRegressor.ModelParameters) throws

Creates a Boosted Tree Regressor from the feature columns in the training data to predict the values in the target column.

Deprecated

struct ModelParameters

Parameters that affect the process of training a model.

let modelParameters: MLBoostedTreeRegressor.ModelParameters

The underlying parameters used when training the model.

var targetColumn: String

The name of the column you selected at initialization to define which feature the regressor predicts.

var featureColumns: [String]

The names of the columns you selected at initialization to train the regressor.

### Assessing model accuracy

var trainingMetrics: MLRegressorMetrics

Measurements of the regressor’s performance on the training data set.

var validationMetrics: MLRegressorMetrics

Measurements of the regressor’s performance on the validation data set.

### Evaluating a boosted tree regressor

func evaluation(on: DataFrame) -> MLRegressorMetrics

Evaluates the classifier on the provided labeled data.

func evaluation(on: MLDataTable) -> MLRegressorMetrics

Evaluates the classifier on the provided labeled data.

Deprecated

### Testing a boosted tree regressor

func predictions(from: DataFrame) throws -> AnyColumn

Predicts a column of labels for the given testing data.

func predictions(from: MLDataTable) throws -> MLUntypedColumn

Predicts the target value from the provided data.

Deprecated

### Saving a boosted tree regressor

func write(to: URL, metadata: MLModelMetadata?) throws

Exports a Core ML model file for use in your app.

func write(toFile: String, metadata: MLModelMetadata?) throws

Exports a Core ML model file for use in your app.

### Describing a boosted tree regressor

var model: MLModel

The Core ML model.

var description: String

A text representation of the boosted tree regressor.

var debugDescription: String

A text representation of the boosted tree regressor that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the boosted tree regressor shown in a playground.

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

struct MLLinearRegressor

A regressor that estimates the target as a linear function of the features.

struct MLDecisionTreeRegressor

A regressor that estimates the target by learning rules to split the data.

struct MLRandomForestRegressor

A regressor based on a collection of decision trees trained on subsets of the data.

