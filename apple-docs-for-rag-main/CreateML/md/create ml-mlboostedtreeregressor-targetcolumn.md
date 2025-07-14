

- Create ML
- MLBoostedTreeRegressor
-  targetColumn 

Instance Property

# targetColumn

The name of the column you selected at initialization to define which feature the regressor predicts.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
var targetColumn: String
```

## Discussion

Changing the value of this property doesn’t retrain the model or affect its behavior.

## See Also

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

var featureColumns: [String]

The names of the columns you selected at initialization to train the regressor.

