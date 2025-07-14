

- Create ML Components
- MultiLabelClassificationMetrics
-  meanAveragePrecision 

Instance Property

# meanAveragePrecision

The mean average precision.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
var meanAveragePrecision: Float { get }
```

## Discussion

An average precision score summarizes the precision-recall curve for a label. The mean average precision is the mean of the average precision scores for all the classification labels.

## See Also

### Getting the properties

var confidenceThresholds: [Label : Float]

A dictionary of label and confidence thresholds.

var exampleCount: Int

The number of examples used to compute the metrics.

var labels: Set&lt;Label>

The classifier labels.

