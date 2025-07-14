

- Create ML
- MLRandomForestRegressor
-  init(trainingData:targetColumn:featureColumns:parameters:) Deprecated

Initializer

# init(trainingData:targetColumn:featureColumns:parameters:)

Creates a Random Forest Regressor from the feature columns in the training data to predict the values in the target column.

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedMac Catalyst 15.0–16.0DeprecatedmacOS 10.14–13.0DeprecatedvisionOS 1.0+

``` source
init(
    trainingData: MLDataTable,
    targetColumn: String,
    featureColumns: [String]? = nil,
    parameters: MLRandomForestRegressor.ModelParameters = ModelParameters(validationData: nil)
) throws
```

Deprecated

Use DataFrame instead of MLDataTable when initializing.

## Parameters 

`trainingData`  

A data table of training examples.

`targetColumn`  

The column name for the values in the training data the regressor should predict.

`featureColumns`  

The column names for the values in the training data that the regressor uses to predict the target value.

`parameters`  

The model parameters.

## See Also

### Creating and Training a Random Forest Regressor

init(checkpoint: MLCheckpoint) throws

Creates a random forest regressor from a checkpoint.

init(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLRandomForestRegressor.ModelParameters) throws

Creates a random tree regressor.

static func makeTrainingSession(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLRandomForestRegressor.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLRandomForestRegressor>

Creates or restores a training session.

static func makeTrainingSession(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLRandomForestRegressor.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLRandomForestRegressor>

Creates or restores a training session.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLRandomForestRegressor>

Restores an existing training session.

static func resume(MLTrainingSession&lt;MLRandomForestRegressor>) throws -> MLJob&lt;MLRandomForestRegressor>

Resumes a training session from the last checkpoint if available.

static func train(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLRandomForestRegressor.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLRandomForestRegressor>

Trains a random forest regressor.

static func train(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLRandomForestRegressor.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLRandomForestRegressor>

Trains a random forest regressor.

struct ModelParameters

Parameters that affect the process of training a model.

let modelParameters: MLRandomForestRegressor.ModelParameters

The underlying parameters used when training the model.

var targetColumn: String

The name of the column you selected at initialization to define which feature the regressor predicts.

var featureColumns: [String]

The names of the columns you selected at initialization to train the regressor.

