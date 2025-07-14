

- Create ML
- MLDecisionTreeRegressor
-  init(trainingData:targetColumn:featureColumns:parameters:) 

Initializer

# init(trainingData:targetColumn:featureColumns:parameters:)

Creates a decision tree regressor.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
init(
    trainingData: DataFrame,
    targetColumn: String,
    featureColumns: [String]? = nil,
    parameters: MLDecisionTreeRegressor.ModelParameters = ModelParameters(validation: .split(strategy: .automatic))
) throws
```

## Parameters 

`trainingData`  

The training data

`targetColumn`  

Name of the column containing the target values

`featureColumns`  

Names of the columns containing feature values. If `nil` all columns, other than the target column, will be used as feature values.

`parameters`  

Model training parameters

## See Also

### Creating and training a decision tree regressor

init(checkpoint: MLCheckpoint) throws

Creates a decision tree regressor from a checkpoint.

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

struct ModelParameters

Parameters that affect the process of training a model.

let modelParameters: MLDecisionTreeRegressor.ModelParameters

The underlying parameters used when training the model.

var targetColumn: String

The name of the column you selected at initialization to define which feature the regressor predicts.

var featureColumns: [String]

The names of the columns you selected at initialization to train the regressor.

