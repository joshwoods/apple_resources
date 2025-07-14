

- Create ML
- MLLogisticRegressionClassifier
-  init(trainingData:targetColumn:featureColumns:parameters:) Deprecated

Initializer

# init(trainingData:targetColumn:featureColumns:parameters:)

Creates a Logistic Regression Classifier from the feature columns in the training data to predict the categories in the target column.

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedMac Catalyst 15.0–16.0DeprecatedmacOS 10.14–13.0DeprecatedvisionOS 1.0+

``` source
init(
    trainingData: MLDataTable,
    targetColumn: String,
    featureColumns: [String]? = nil,
    parameters: MLLogisticRegressionClassifier.ModelParameters = ModelParameters(validationData: nil)
) throws
```

Deprecated

Use DataFrame instead of MLDataTable when initializing.

## Parameters 

`trainingData`  

A data table of training examples.

`targetColumn`  

The column name for the values in the training data that the classifier should predict.

`featureColumns`  

The column names for the values in the training data that the classifier uses to predict the target value.

`parameters`  

The model parameters.

## See Also

### Creating and training a logistic regression classifier

init(checkpoint: MLCheckpoint) throws

Creates a logistic regression classifier from a checkpoint.

init(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLLogisticRegressionClassifier.ModelParameters) throws

Creates a logistic regression classifier.

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

var featureColumns: [String]

The names of the columns you selected at initialization to train the classifier.

