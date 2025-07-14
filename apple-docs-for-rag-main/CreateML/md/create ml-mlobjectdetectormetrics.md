

- Create ML
-  MLObjectDetectorMetrics 

Structure

# MLObjectDetectorMetrics

Metrics you use to evaluate an object detector’s performance.

macOS 10.15+

``` source
struct MLObjectDetectorMetrics
```

## Overview

An object detector generates intersection-over-union (IoU) metrics, which is a way to measure the similarity of two bounding boxes. The IoU metric is the overlapping area divided by the area of the union of the bounding boxes.

For example, two bounding boxes that overlap perfectly have an IoU of `1.0`, because their overlap is the same area as the union. Two bounding boxes that have no overlap have an IoU of `0.0`. Anything between `0.0` and `1.0` either means the two bounding boxes partially overlap or one box completely encases the other.

## Topics

### Creating metrics

init(averagePrecision: (variedIoU: [String : Double], IoU50: [String : Double]), meanAveragePrecision: (variedIoU: Double, IoU50: Double))

Creates metrics for an object detector given an average precision and a mean average precision.

### Assessing the model

var averagePrecision: (variedIoU: [String : Double], IoU50: [String : Double])

Two dictionaries of average precisions at different thresholds.

var meanAveragePrecision: (variedIoU: Double, IoU50: Double)

Two mean-average precisions at different thresholds.

### Handling errors

var isValid: Bool

A Boolean value indicating whether the object detector model was able to calculate metrics.

var error: (any Error)?

The underlying error present when the metrics are invalid.

### Describing metrics

var description: String

A text representation of the object detector metrics.

var debugDescription: String

A text representation of the object detector metrics that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the object detector metrics shown in a playground.

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

### Model Accuracy

Improving Your Model’s Accuracy

Use metrics to tune the performance of your machine learning model.

struct MLClassifierMetrics

Metrics you use to evaluate a classifier’s performance.

struct MLRegressorMetrics

Metrics you use to evaluate a regressor’s performance.

struct MLWordTaggerMetrics

Metrics you use to evaluate a word tagger’s performance.

struct MLRecommenderMetrics

Metrics you use to evaluate a recommender’s performance.

