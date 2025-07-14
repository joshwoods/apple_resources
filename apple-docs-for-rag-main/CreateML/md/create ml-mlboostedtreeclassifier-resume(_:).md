

- Create ML
- MLBoostedTreeClassifier
-  resume(\_:) 

Type Method

# resume(\_:)

Resumes a training session from the last checkpoint if available.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
static func resume(_ session: MLTrainingSession) throws -> MLJob
```

## Parameters 

`session`  

Loaded or new training session.

## Return Value

A `MLJob` that can be used to observe training progress.

## Discussion

If there are no resumable checkpoints training starts over from the beginning.

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

static func train(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLBoostedTreeClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLBoostedTreeClassifier>

Trains a boosted tree classifier.

static func train(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLBoostedTreeClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLBoostedTreeClassifier>

Trains a boosted tree classifier.

init(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLBoostedTreeClassifier.ModelParameters) throws

Creates a Boosted Tree Classifier from the feature columns in the training data to predict the categories in the target column.

Deprecated

struct ModelParameters

Parameters that affect the process of training a model.

let modelParameters: MLBoostedTreeClassifier.ModelParameters

The underlying parameters used when training the model.

var targetColumn: String

The name of the column you selected at initialization to define which categories the classifier predicts.

var featureColumns: [String]

The names of the columns you selected at initialization to train the classifier.

