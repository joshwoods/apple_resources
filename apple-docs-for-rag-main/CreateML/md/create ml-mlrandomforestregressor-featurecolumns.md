

- Create ML
- MLRandomForestRegressor
-  featureColumns 

Instance Property

# featureColumns

The names of the columns you selected at initialization to train the regressor.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
var featureColumns: [String]
```

## Discussion

Changing the value of this property doesn’t retrain the model or affect its behavior.

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

init(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLRandomForestRegressor.ModelParameters) throws

Creates a Random Forest Regressor from the feature columns in the training data to predict the values in the target column.

Deprecated

struct ModelParameters

Parameters that affect the process of training a model.

let modelParameters: MLRandomForestRegressor.ModelParameters

The underlying parameters used when training the model.

var targetColumn: String

The name of the column you selected at initialization to define which feature the regressor predicts.

