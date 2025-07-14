

- Create ML
- MLBoostedTreeRegressor
-  makeTrainingSession(trainingData:targetColumn:featureColumns:parameters:sessionParameters:) 

Type Method

# makeTrainingSession(trainingData:targetColumn:featureColumns:parameters:sessionParameters:)

Creates or restores a training session.

iOS 15.0–17.0DeprecatediPadOS 15.0–17.0DeprecatedMac Catalyst 15.0–17.0DeprecatedmacOS 12.0–14.0DeprecatedtvOS 16.0–17.0DeprecatedvisionOS 1.0+

``` source
static func makeTrainingSession(
    trainingData: MLDataTable,
    targetColumn: String,
    featureColumns: [String]? = nil,
    parameters: MLBoostedTreeRegressor.ModelParameters = ModelParameters(validation: .split(strategy: .automatic)),
    sessionParameters: MLTrainingSessionParameters = _defaultSessionParameters
) throws -> MLTrainingSession
```

## Parameters 

`trainingData`  

A DataTable specifying training data.

`targetColumn`  

A String specifying the target column name in the trainingData

`featureColumns`  

An optional list of Strings specifying feature columns to be used to predict the target, if not provided, default to use all the other columns in the trainingData, except the one specified by targetColumn

`parameters`  

Model training parameters. See `MLBoostedTreeRegressor.ModelParameters` for the defaults.

`sessionParameters`  

Training session parameters. See `MLTrainingSessionParameters` for the defaults.

## Return Value

A `MLTrainingSession` that can be used to start or resume training.

## See Also

### Creating and training a boosted tree regressor

init(checkpoint: MLCheckpoint) throws

Creates a boosted tree regressor from a checkpoint.

init(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLBoostedTreeRegressor.ModelParameters) throws

Creates a boosted tree regressor.

static func makeTrainingSession(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLBoostedTreeRegressor.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLBoostedTreeRegressor>

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

