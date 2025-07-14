

- Create ML
-  MLClassifierMetrics 

Structure

# MLClassifierMetrics

Metrics you use to evaluate a classifier’s performance.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
struct MLClassifierMetrics
```

## Mentioned in 

Creating a Text Classifier Model

Creating a text classifier model

Creating an Image Classifier Model

Improving Your Model’s Accuracy

## Overview

Use MLClassifierMetrics to evaluate your model’s ability to distinguish between different categories when it’s classifying data.

You can determine the model’s accuracy using the classificationError metric. For information about how your model is mislabeling or missing a certain category, use the precisionRecall metric. To determine specific cases where your model is mistaking one label for another, use the confusion property.

Accuracy can be a misleading metric if you use unbalanced data, which means the number of examples for some categories are much larger than others. Instead, use precisionRecall or confusion.

Note

Each trained model contains different metrics for its various data sets (training, validation, and testing). Improving Your Model’s Accuracy compares these metrics between different data sets.

## Topics

### Understanding the model

var classificationError: Double

The fraction of incorrectly labeled examples.

var precisionRecall: MLDataTable

A data table listing the precision and recall percentages for each class.

var confusion: MLDataTable

A table comparing the actual and predicted labels for each classification category.

var confusionDataFrame: DataFrame

A data frame comparing the actual and predicted labels for each class.

var precisionRecallDataFrame: DataFrame

A data frame listing the precision and recall percentages for each class.

### Handling errors

var isValid: Bool

A Boolean value indicating whether the classifier model was able to calculate metrics.

var error: (any Error)?

The underlying error present when the metrics are invalid.

### Creating metrics

init(classificationError: Double, confusion: MLDataTable, precisionRecall: MLDataTable)

Creates empty classifier metrics.

### Describing metrics

var description: String

A text representation of the classifier metrics.

var debugDescription: String

A text representation of the classifier metrics that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the classifier metrics shown in a playground.

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

### Model Accuracy

Improving Your Model’s Accuracy

Use metrics to tune the performance of your machine learning model.

struct MLRegressorMetrics

Metrics you use to evaluate a regressor’s performance.

struct MLWordTaggerMetrics

Metrics you use to evaluate a word tagger’s performance.

struct MLRecommenderMetrics

Metrics you use to evaluate a recommender’s performance.

struct MLObjectDetectorMetrics

Metrics you use to evaluate an object detector’s performance.

