

- Create ML
- MLDecisionTreeRegressor
-  resume(\_:) 

Type Method

# resume(\_:)

Resumes a training session from the last checkpoint if available.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
static func resume(_ session: MLTrainingSession) throws -> MLJob
```

## Parameters 

`session`  

Loaded or new training session.

## Return Value

A `MLJob` that can be used to observe training progress.

## Discussion

If there are no resumable checkpoints training starts over from the beginning.

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

static func train(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLDecisionTreeRegressor.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLDecisionTreeRegressor>

Trains a decision tree regressor.

static func train(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLDecisionTreeRegressor.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLDecisionTreeRegressor>

Trains a decision tree regressor.

init(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLDecisionTreeRegressor.ModelParameters) throws

Creates a Decision Tree Regressor from the feature columns in the training data to predict the values in the target column.

Deprecated

struct ModelParameters

Parameters that affect the process of training a model.

let modelParameters: MLDecisionTreeRegressor.ModelParameters

The underlying parameters used when training the model.

var targetColumn: String

The name of the column you selected at initialization to define which feature the regressor predicts.

var featureColumns: [String]

The names of the columns you selected at initialization to train the regressor.

