

- Create ML
-  MLRecommenderMetrics 

Structure

# MLRecommenderMetrics

Metrics you use to evaluate a recommender’s performance.

macOS 10.15+

``` source
struct MLRecommenderMetrics
```

## Topics

### Assessing the model

let excludingObserved: Bool

A Boolean value that indicates whether the recommender omitted training data from the recommendations.

var precisionRecall: MLDataTable

A data table with the recall and precision for each item.

Deprecated

var precisionRecallDataFrame: DataFrame

A data table with the recall and precision for each item.

### Handling errors

var isValid: Bool

A Boolean value indicating whether the recommender model was able to calculate metrics.

let error: (any Error)?

The underlying error present when the metrics are invalid.

### Creating metrics

init(precisionRecall: MLDataTable, excludingObserved: Bool)

Creates metrics for a recommender, given a data table with precision and recall metric columns, and whether the recommender omitted training data.

Deprecated

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

struct MLObjectDetectorMetrics

Metrics you use to evaluate an object detector’s performance.

