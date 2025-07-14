

- Create ML
- MLBoostedTreeRegressor
-  MLBoostedTreeRegressor.ModelParameters 

Structure

# MLBoostedTreeRegressor.ModelParameters

Parameters that affect the process of training a model.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
struct ModelParameters
```

## Topics

### Creating parameters

init(validation: MLBoostedTreeRegressor.ModelParameters.ValidationData, maxDepth: Int, maxIterations: Int, minLossReduction: Double, minChildWeight: Double, randomSeed: Int, stepSize: Double, earlyStoppingRounds: Int?, rowSubsample: Double, columnSubsample: Double)

init(validationData: MLDataTable?, maxDepth: Int, maxIterations: Int, minLossReduction: Double, minChildWeight: Double, randomSeed: Int, stepSize: Double, earlyStoppingRounds: Int?, rowSubsample: Double, columnSubsample: Double)

Creates a new set of parameters.

Deprecated

enum ValidationData

Values for specifying validation data.

### Accessing parameters

var columnSubsample: Double

Must be in the range (0, 1).

var earlyStoppingRounds: Int?

Validation data must be specified for an early stop.

var maxDepth: Int

var maxIterations: Int

var minChildWeight: Double

var minLossReduction: Double

var randomSeed: Int

var rowSubsample: Double

Must be in the range (0, 1).

var stepSize: Double

Must be in the range (0, 1).

var validationData: MLDataTable?

Validation data represented as a `MLDataTable`.

Deprecated

var validation: MLBoostedTreeRegressor.ModelParameters.ValidationData

Validation data.

### Describing parameters

var description: String

A text representation of the model parameters for a boosted tree regressor.

var debugDescription: String

A text representation of the model parameters for a boosted tree regressor that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the model parameters for a boosted tree regressor shown in a playground.

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

let modelParameters: MLBoostedTreeRegressor.ModelParameters

The underlying parameters used when training the model.

var targetColumn: String

The name of the column you selected at initialization to define which feature the regressor predicts.

var featureColumns: [String]

The names of the columns you selected at initialization to train the regressor.

