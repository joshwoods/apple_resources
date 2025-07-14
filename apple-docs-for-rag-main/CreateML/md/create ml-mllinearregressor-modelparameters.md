

- Create ML
- MLLinearRegressor
-  modelParameters 

Instance Property

# modelParameters

The underlying parameters used when training the model.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
let modelParameters: MLLinearRegressor.ModelParameters
```

## See Also

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

var targetColumn: String

The name of the column you selected at initialization to define which feature the regressor predicts.

var featureColumns: [String]

The names of the columns you selected at initialization to train the regressor.

