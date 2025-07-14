

- Create ML
-  MLLogisticRegressionClassifier 

Structure

# MLLogisticRegressionClassifier

A classifier that predicts a discrete target value as a function of data features.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
struct MLLogisticRegressionClassifier
```

## Topics

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

var featureColumns: [String]

The names of the columns you selected at initialization to train the classifier.

### Assessing model accuracy

var trainingMetrics: MLClassifierMetrics

Measurements of the classifier’s performance on the training data set.

var validationMetrics: MLClassifierMetrics

Measurements of the classifier’s performance on the validation data set.

### Evaluating a logistic regression classifier

func evaluation(on: DataFrame) -> MLClassifierMetrics

Evaluates the classifier on the provided labeled data.

func evaluation(on: MLDataTable) -> MLClassifierMetrics

Evaluates the classifier on the provided labeled data.

Deprecated

### Testing a logistic regression classifier

func predictions(from: DataFrame) throws -> AnyColumn

Predicts a column of labels for the given testing data.

func predictions(from: MLDataTable) throws -> MLUntypedColumn

Classifies the provided data into the target categories.

Deprecated

### Saving a logistic regression classifier

func write(to: URL, metadata: MLModelMetadata?) throws

Exports a Core ML model file for use in your app.

func write(toFile: String, metadata: MLModelMetadata?) throws

Exports a Core ML model file for use in your app.

### Describing a logistic regression classifier

var model: MLModel

The Core ML model.

var description: String

A text representation of the logistic regression classifier.

var debugDescription: String

A text representation of the logistic regression classifier that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the logistic regression classifier shown in a playground.

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
- Sendable

## See Also

### Supporting classifier types

struct MLDecisionTreeClassifier

A classifier that predicts the target by creating rules to split the data.

struct MLRandomForestClassifier

A classifier based on a collection of decision trees trained on subsets of the data.

struct MLBoostedTreeClassifier

A classifier based on a collection of decision trees combined with gradient boosting.

struct MLSupportVectorClassifier

A classifier that predicts a binary target value by maximizing the separation between categories.

Deprecated

