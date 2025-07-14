

- Create ML
- MLLogisticRegressionClassifier
-  featureColumns 

Instance Property

# featureColumns

The names of the columns you selected at initialization to train the classifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
var featureColumns: [String]
```

## Discussion

Changing the value of this property doesn’t retrain the model or affect its behavior.

## See Also

### Creating and training a logistic regression classifier

init(checkpoint: MLCheckpoint) throws

Creates a logistic regression classifier from a checkpoint.

init(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLLogisticRegressionClassifier.ModelParameters) throws

Creates a logistic regression classifier.

init(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLLogisticRegressionClassifier.ModelParameters) throws

Creates a Logistic Regression Classifier from the feature columns in the training data to predict the categories in the target column.

Deprecated

static func train(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLLogisticRegressionClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLLogisticRegressionClassifier>

Trains a logistic regression classifier.

static func train(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLLogisticRegressionClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLJob&lt;MLLogisticRegressionClassifier>

Trains a logistic regression classifier.

static func makeTrainingSession(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLLogisticRegressionClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLLogisticRegressionClassifier>

Creates or restores a training session.

static func makeTrainingSession(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLLogisticRegressionClassifier.ModelParameters, sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLLogisticRegressionClassifier>

Creates or restores a training session.

static func resume(MLTrainingSession&lt;MLLogisticRegressionClassifier>) throws -> MLJob&lt;MLLogisticRegressionClassifier>

Resumes a training session from the last checkpoint if available.

static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession&lt;MLLogisticRegressionClassifier>

Restores an existing training session.

struct ModelParameters

Parameters that affect the process of training a model.

let modelParameters: MLLogisticRegressionClassifier.ModelParameters

The underlying parameters used when training the model.

var targetColumn: String

The name of the column you selected at initialization to define which categories the classifier predicts.

