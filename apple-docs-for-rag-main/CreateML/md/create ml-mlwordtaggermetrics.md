

- Create ML
-  MLWordTaggerMetrics 

Structure

# MLWordTaggerMetrics

Metrics you use to evaluate a word tagger’s performance.

macOS 10.14+

``` source
struct MLWordTaggerMetrics
```

## Topics

### Analyzing the tagger’s performance

var taggingError: Double

The fraction of incorrectly tagged examples.

var precisionRecall: MLDataTable

A data table listing the precision and recall percentages for each category.

Deprecated

var confusion: MLDataTable

A table comparing the actual and predicted labels for each tagging category.

Deprecated

### Handling errors

var isValid: Bool

A Boolean value indicating whether the metrics were calculated.

var error: (any Error)?

The underlying error present when the metrics are invalid.

### Describing metrics

var description: String

A text representation of the word tagger metrics.

var debugDescription: String

A text representation of the word tagger metrics that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the word tagger metrics shown in a playground.

### Instance Properties

var confusionDataFrame: DataFrame

A data frame comparing the actual and predicted labels for each class.

var precisionRecallDataFrame: DataFrame

A data frame listing the precision and recall percentages for each class.

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

struct MLClassifierMetrics

Metrics you use to evaluate a classifier’s performance.

struct MLRegressorMetrics

Metrics you use to evaluate a regressor’s performance.

struct MLRecommenderMetrics

Metrics you use to evaluate a recommender’s performance.

struct MLObjectDetectorMetrics

Metrics you use to evaluate an object detector’s performance.

