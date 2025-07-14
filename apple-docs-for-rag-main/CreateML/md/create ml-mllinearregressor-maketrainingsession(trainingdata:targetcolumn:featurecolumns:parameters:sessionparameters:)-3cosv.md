

- Create ML
- MLLinearRegressor
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
    parameters: MLLinearRegressor.ModelParameters = ModelParameters(validation: .split(strategy: .automatic)),
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

Model training parameters. See `MLLinearRegressor.ModelParameters` for the defaults.

`sessionParameters`  

Training session parameters. See `MLTrainingSessionParameters` for the defaults.

## Return Value

A `MLTrainingSession` that can be used to start or resume training.

## See Also

### Creating and Training a Linear Regressor

init(checkpoint: MLCheckpoint) throws

Creates a linear regressor from a checkpoint.

init(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLLinearRegressor.ModelParameters) throws

Creates a linear regressor.

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

