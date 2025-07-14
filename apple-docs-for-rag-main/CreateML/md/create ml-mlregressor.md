

- Create ML
-  MLRegressor 

Enumeration

# MLRegressor

A model you train to estimate continuous values.

macOS 10.14+

``` source
enum MLRegressor
```

## Mentioned in 

Improving Your Model’s Accuracy

## Overview

Use an MLRegressor to estimate continuous values like price, time, or temperature.

A regressor differs from a classifier because it can predict output values not seen during the training process. By contrast, a classifier can only classify input into the categories you provide in the training data.

For example, when estimating housing prices on Mars, a regressor can interpolate between the examples to estimate prices not seen during training. The figure below shows a linear regressor for Mars real-estate prices similar to the Integrating a Core ML Model into Your App sample.

In this case, there are no data points with three solar panels, but the regressor can make an informed prediction about the housing price.

When you create an MLRegressor, Create ML inspects your data and automatically chooses a specific regressor (see *Supporting Regressor Types*).

## Topics

### Creating and training a regressor

init(trainingData: DataFrame, targetColumn: String, featureColumns: [String]?) throws

Creates a regressor.

init(trainingData: MLDataTable, targetColumn: String, featureColumns: [String]?) throws

Creates a regressor from the feature columns in the training data to predict the values in the target column.

Deprecated

var targetColumn: String

The name of the column you selected at initialization to define which feature the regressor predicts.

var featureColumns: [String]

The names of the columns you selected at initialization to train the regressor.

### Assessing model accuracy

var trainingMetrics: MLRegressorMetrics

Measurements of the regressor’s performance on the training data set.

var validationMetrics: MLRegressorMetrics

Measurements of the regressor’s performance on the validation data set.

### Evaluating a regressor

func evaluation(on: DataFrame) -> MLRegressorMetrics

Evaluates the classifier on the provided labeled data.

func evaluation(on: MLDataTable) -> MLRegressorMetrics

Evaluates the classifier on the provided labeled data.

Deprecated

### Testing a regressor

func predictions(from: DataFrame) throws -> AnyColumn

func predictions(from: MLDataTable) throws -> MLUntypedColumn

Predicts the target value from the provided data.

Deprecated

### Saving a regressor

func write(to: URL, metadata: MLModelMetadata?) throws

Exports a Core ML model file for use in your app.

func write(toFile: String, metadata: MLModelMetadata?) throws

Exports a Core ML model file for use in your app.

### Describing a regressor

var model: MLModel

The underlying Core ML model stored in memory.

var description: String

A text representation of the regressor.

var debugDescription: String

A text representation of the regressor that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the regressor shown in a playground.

### Regressor cases

case linear(MLLinearRegressor)

A regressor that estimates the target as a linear function of the features.

case decisionTree(MLDecisionTreeRegressor)

A regressor that estimates the target by learning rules to split the data.

case boostedTree(MLBoostedTreeRegressor)

A regressor based on a collection of decision trees combined with gradient boosting.

case randomForest(MLRandomForestRegressor)

A regressor based on a collection of decision trees trained on subsets of the data.

### Supporting regressor types

struct MLLinearRegressor

A regressor that estimates the target as a linear function of the features.

struct MLDecisionTreeRegressor

A regressor that estimates the target by learning rules to split the data.

struct MLRandomForestRegressor

A regressor based on a collection of decision trees trained on subsets of the data.

struct MLBoostedTreeRegressor

A regressor based on a collection of decision trees combined with gradient boosting.

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

enum MLClassifier

A model you train to classify data into discrete categories.

struct MLRecommender

A model you train to make recommendations based on item similarity, grouping, and, optionally, item ratings.

