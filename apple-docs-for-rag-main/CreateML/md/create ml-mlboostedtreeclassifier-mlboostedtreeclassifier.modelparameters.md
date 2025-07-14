

- Create ML
- MLBoostedTreeClassifier
-  MLBoostedTreeClassifier.ModelParameters 

Structure

# MLBoostedTreeClassifier.ModelParameters

Parameters that affect the process of training a model.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
struct ModelParameters
```

## Topics

### Creating parameters

init(validation: MLBoostedTreeClassifier.ModelParameters.ValidationData, maxDepth: Int, maxIterations: Int, minLossReduction: Double, minChildWeight: Double, randomSeed: Int, stepSize: Double, earlyStoppingRounds: Int?, rowSubsample: Double, columnSubsample: Double)

init(validationData: MLDataTable?, maxDepth: Int, maxIterations: Int, minLossReduction: Double, minChildWeight: Double, randomSeed: Int, stepSize: Double, earlyStoppingRounds: Int?, rowSubsample: Double, columnSubsample: Double)

Creates a new set of parameters defining how a boosted tree classifier should be built.

Deprecated

enum ValidationData

Values for specifying validation data.

### Accessing parameters

var validationData: MLDataTable?

Validation data represented as a `MLDataTable`.

Deprecated

var maxDepth: Int

var maxIterations: Int

var minLossReduction: Double

var minChildWeight: Double

var randomSeed: Int

var stepSize: Double

Must be in the range (0, 1).

var earlyStoppingRounds: Int?

Validation data must be specified for an early stop.

var rowSubsample: Double

Must be in the range (0, 1).

var columnSubsample: Double

Must be in the range (0, 1).

var validation: MLBoostedTreeClassifier.ModelParameters.ValidationData

Validation data.

### Describing parameters

var description: String

A text representation of the model parameters for a boosted tree classifier.

var debugDescription: String

A text representation of the model parameters for a boosted tree classifier that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the model parameters for a boosted tree classifier shown in a playground.

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

### Creating and training a boosted tree classifier

init(checkpoint: MLCheckpoint) throws

Creates a boosted tree classifier from a checkpoint.

init(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLBoostedTreeClassifier.ModelParameters) throws

Creates a boosted tree classifier.

static func makeTrainingSession(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLBoostedTreeClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLBoostedTreeClassifier>

Creates or restores a training session.

static func makeTrainingSession(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLBoostedTreeClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLBoostedTreeClassifier>

Creates or restores a training session.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLBoostedTreeClassifier>

Restores an existing training session.

static func resume(MLTrainingSession&lt;MLBoostedTreeClassifier>) throws -> MLJob&lt;MLBoostedTreeClassifier>

Resumes a training session from the last checkpoint if available.

static func train(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLBoostedTreeClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLBoostedTreeClassifier>

Trains a boosted tree classifier.

static func train(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLBoostedTreeClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLBoostedTreeClassifier>

Trains a boosted tree classifier.

init(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLBoostedTreeClassifier.ModelParameters) throws

Creates a Boosted Tree Classifier from the feature columns in the training data to predict the categories in the target column.

Deprecated

let modelParameters: MLBoostedTreeClassifier.ModelParameters

The underlying parameters used when training the model.

var targetColumn: String

The name of the column you selected at initialization to define which categories the classifier predicts.

var featureColumns: [String]

The names of the columns you selected at initialization to train the classifier.

