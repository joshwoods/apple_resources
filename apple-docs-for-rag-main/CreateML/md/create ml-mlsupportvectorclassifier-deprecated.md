

- Create ML
-  MLSupportVectorClassifier Deprecated

Structure

# MLSupportVectorClassifier

A classifier that predicts a binary target value by maximizing the separation between categories.

macOS 10.14–14.0Deprecated

``` source
struct MLSupportVectorClassifier
```

## Topics

### Creating and training a support vector classifier

init(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?, parameters: MLSupportVectorClassifier.ModelParameters) throws

Creates a support vector classifier.

init(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?, parameters: MLSupportVectorClassifier.ModelParameters) throws

Creates a Support Vector Classifier from the feature columns in the training data to predict the categories in the target column.

struct ModelParameters

Parameters that affect the process of training a model.

let modelParameters: MLSupportVectorClassifier.ModelParameters

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

### Evaluating a support vector classifier

func evaluation(on: DataFrame) -> MLClassifierMetrics

Evaluates the classifier on the provided labeled data.

func evaluation(on: MLDataTable) -> MLClassifierMetrics

Evaluates the classifier on the provided labeled data.

### Testing a support vector classifier

func predictions(from: DataFrame) throws -> AnyColumn

Predicts a column of labels for the given testing data.

func predictions(from: MLDataTable) throws -> MLUntypedColumn

Classifies the provided data into the target categories.

### Saving a support vector classifier

func write(to: URL, metadata: MLModelMetadata?) throws

Exports a Core ML model file for use in your app.

func write(toFile: String, metadata: MLModelMetadata?) throws

Exports a Core ML model file for use in your app.

### Describing a support vector classifier

var model: MLModel

The Core ML model.

var description: String

A text representation of the support vector classifier.

var debugDescription: String

A text representation of the support vector classifier that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the support vector classifier shown in a playground.

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

struct MLLogisticRegressionClassifier

A classifier that predicts a discrete target value as a function of data features.

