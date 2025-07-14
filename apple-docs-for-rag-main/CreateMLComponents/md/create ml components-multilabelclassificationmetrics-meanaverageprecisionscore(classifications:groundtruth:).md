

- Create ML Components
- MultiLabelClassificationMetrics
-  meanAveragePrecisionScore(classifications:groundTruth:) 

Type Method

# meanAveragePrecisionScore(classifications:groundTruth:)

Computes the mean average precision.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
static func meanAveragePrecisionScore(
    classifications: some Sequence>,
    groundTruth: some Sequence>
) -> Float
```

Available when `Label` conforms to `Hashable`.

## Parameters 

`classifications`  

A sequence of multi-label classifications.

`groundTruth`  

A sequence of multi-label correct labels.

## Return Value

The mean average precision.

## Discussion

An average precision score summarizes the precision-recall curve for a label. The mean average precision is the mean of the average precision scores for all the classification labels.

## See Also

### Computing the precision

static func meanAveragePrecisionScore(some Sequence&lt;(classification: ClassificationDistribution&lt;Label>, labels: Set&lt;Label>)>) -> Float

Computes the mean average precision.

static func meanAveragePrecisionScore(some Sequence&lt;(classification: ClassificationDistribution&lt;Label>, labels: Set&lt;Label>)>, labels: Set&lt;Label>) -> Float

Computes the mean average precision.

static func meanAveragePrecisionScore(classifications: some Sequence&lt;ClassificationDistribution&lt;Label>>, groundTruth: some Sequence&lt;Set&lt;Label>>, labels: Set&lt;Label>) -> Float

Computes the mean average precision.

