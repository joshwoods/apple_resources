

- Create ML
-  MLBoostedTreeClassifier 

Structure

# MLBoostedTreeClassifier

A classifier based on a collection of decision trees combined with gradient boosting.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
struct MLBoostedTreeClassifier
```

## Overview

A boosted tree classifier combines several MLDecisionTreeClassifier models (a technique known as *ensemble learning*) by training each model to correct the errors of the preceding model.

This model is useful for handling numerical and categorical features, but is less suitable for sparse data such as text.

## Topics

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

struct ModelParameters

Parameters that affect the process of training a model.

let modelParameters: MLBoostedTreeClassifier.ModelParameters

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

### Evaluating the boosted tree classifier

func evaluation(on: DataFrame) -> MLClassifierMetrics

Evaluates the classifier on the provided labeled data.

func evaluation(on: MLDataTable) -> MLClassifierMetrics

Evaluates the classifier on the provided labeled data.

Deprecated

### Testing a boosted tree classifier

func predictions(from: DataFrame) throws -> AnyColumn

Predicts a column of labels for the given testing data.

func predictions(from: MLDataTable) throws -> MLUntypedColumn

Classifies the provided data into the target categories.

Deprecated

### Saving a boosted tree classifier

func write(to: URL, metadata: MLModelMetadata?) throws

Exports a Core ML model file for use in your app.

func write(toFile: String, metadata: MLModelMetadata?) throws

Exports a Core ML model file for use in your app.

### Describing a boosted tree classifier

var model: MLModel

The Core ML model.

var description: String

A text representation of the boosted tree classifier.

var debugDescription: String

A text representation of the boosted tree classifier that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the boosted tree classifier shown in a playground.

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

struct MLLogisticRegressionClassifier

A classifier that predicts a discrete target value as a function of data features.

struct MLSupportVectorClassifier

A classifier that predicts a binary target value by maximizing the separation between categories.

Deprecated

