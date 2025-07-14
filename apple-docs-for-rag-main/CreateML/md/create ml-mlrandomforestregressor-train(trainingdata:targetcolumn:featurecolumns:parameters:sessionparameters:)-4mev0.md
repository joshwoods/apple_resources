

- Create ML
- MLRandomForestRegressor
-  train(trainingData:targetColumn:featureColumns:parameters:sessionParameters:) 

Type Method

# train(trainingData:targetColumn:featureColumns:parameters:sessionParameters:)

Trains a random forest regressor.

iOS 15.0–17.0DeprecatediPadOS 15.0–17.0DeprecatedMac Catalyst 15.0–17.0DeprecatedmacOS 12.0–14.0DeprecatedtvOS 16.0–17.0DeprecatedvisionOS 1.0+

``` source
static func train(
    trainingData: MLDataTable,
    targetColumn: String,
    featureColumns: [String]? = nil,
    parameters: MLRandomForestRegressor.ModelParameters = ModelParameters(validation: .split(strategy: .automatic)),
    sessionParameters: MLTrainingSessionParameters = _defaultSessionParameters
) throws -> MLJob
```

## Parameters 

`trainingData`  

A DataTable specifying training data.

`targetColumn`  

A String specifying the target column name in the trainingData

`featureColumns`  

An optional list of Strings specifying feature columns to be used to predict the target, if not provided, default to use all the other columns in the trainingData, except the one specified by targetColumn

`parameters`  

Model training parameters. See `MLRandomForestRegressor.ModelParameters` for the defaults.

`sessionParameters`  

Training session parameters. See `MLTrainingSessionParameters` for the defaults.

## Return Value

A `MLJob` that can be used to observe training progress.

## Discussion

If `sessionDirectory` is provided it will save training progress. If there is progress already saved training will resume from the last checkpoint.

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

static func train(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLRandomForestRegressor.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLRandomForestRegressor>

Trains a random forest regressor.

init(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLRandomForestRegressor.ModelParameters) throws

Creates a Random Forest Regressor from the feature columns in the training data to predict the values in the target column.

Deprecated

struct ModelParameters

Parameters that affect the process of training a model.

let modelParameters: MLRandomForestRegressor.ModelParameters

The underlying parameters used when training the model.

var targetColumn: String

The name of the column you selected at initialization to define which feature the regressor predicts.

var featureColumns: [String]

The names of the columns you selected at initialization to train the regressor.

