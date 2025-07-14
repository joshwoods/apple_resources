

- Create ML
-  MLClassifier 

Enumeration

# MLClassifier

A model you train to classify data into discrete categories.

macOS 10.14+

``` source
enum MLClassifier
```

## Mentioned in 

Improving Your Model’s Accuracy

## Overview

Use an MLClassifier to train a general-purpose model to recognize categories.

For example, you can create a classifier that predicts whether a sports team is likely to win or lose its next game by training it with these inputs:

- The team’s win-loss ratio

- The team’s game locations

Important

When working with image or natural language data, don’t use MLClassifier. Instead, use the `MLImageClassifierBuilder` or one of the Natural Language models (MLTextClassifier or MLWordTagger).

When you create an MLClassifier, Create ML inspects your data and automatically chooses a specific classifier (see *Supporting Classifier Types*).

## Topics

### Creating and training a classifier

init(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?) throws

Creates a classifier.

init(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?) throws

Creates a classifier from the feature columns in the training data to predict the categories in the target column.

Deprecated

var targetColumn: String

The name of the column you selected at initialization to define which categories the classifier predicts.

var featureColumns: [String]

The names of the columns you selected at initialization to train the classifier.

### Assessing model accuracy

var trainingMetrics: MLClassifierMetrics

Measurements of the classifier’s performance on the training data set.

var validationMetrics: MLClassifierMetrics

Measurements of the classifier’s performance on the validation data set.

### Evaluating a classifier

func evaluation(on: DataFrame) -> MLClassifierMetrics

Evaluates the classifier on the provided labeled data.

func evaluation(on: MLDataTable) -> MLClassifierMetrics

Evaluates the classifier on the provided labeled data.

Deprecated

### Testing a classifier

func predictions(from: DataFrame) throws -> AnyColumn

func predictions(from: MLDataTable) throws -> MLUntypedColumn

Classifies the provided data into the target categories.

Deprecated

### Saving a classifier

func write(to: URL, metadata: MLModelMetadata?) throws

Exports a Core ML model file for use in your app.

func write(toFile: String, metadata: MLModelMetadata?) throws

Exports a Core ML model file for use in your app.

### Describing a model

var model: MLModel

The underlying Core ML model stored in memory.

var description: String

A text representation of the classifier.

var debugDescription: String

A text representation of the classifier that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the classifier shown in a playground.

### Classifier cases

case decisionTree(MLDecisionTreeClassifier)

A classifier that predicts the target by creating rules to split the data.

case randomForest(MLRandomForestClassifier)

A classifier based on a collection of decision trees trained on subsets of the data.

case boostedTree(MLBoostedTreeClassifier)

A classifier based on a collection of decision trees combined with gradient boosting.

case logisticRegression(MLLogisticRegressionClassifier)

A classifier that predicts a discrete target value as a function of data features.

case supportVector(MLSupportVectorClassifier)

A classifier that predicts a binary target value by maximizing the separation between categories.

Deprecated

### Supporting classifier types

struct MLDecisionTreeClassifier

A classifier that predicts the target by creating rules to split the data.

struct MLRandomForestClassifier

A classifier based on a collection of decision trees trained on subsets of the data.

struct MLBoostedTreeClassifier

A classifier based on a collection of decision trees combined with gradient boosting.

struct MLLogisticRegressionClassifier

A classifier that predicts a discrete target value as a function of data features.

struct MLSupportVectorClassifier

A classifier that predicts a binary target value by maximizing the separation between categories.

Deprecated

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

### Tabular Models

Creating a Model from Tabular Data

Train a machine learning model by using Core ML to import and manage tabular data.

enum MLRegressor

A model you train to estimate continuous values.

struct MLRecommender

A model you train to make recommendations based on item similarity, grouping, and, optionally, item ratings.

