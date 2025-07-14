

- Create ML Components
- MultiLabelClassificationMetrics
-  init(classifications:groundTruth:strategy:labels:) 

Initializer

# init(classifications:groundTruth:strategy:labels:)

Creates multi-label classification metrics for classifications and ground truth labels.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
init(
    classifications: some Sequence>,
    groundTruth: some Sequence>,
    strategy: MultiLabelClassificationMetrics.ThresholdSelectionStrategy,
    labels: Set
) throws
```

## Parameters 

`classifications`  

A sequence of classifications.

`groundTruth`  

A sequence of true labels.

`strategy`  

A label confidence threshold selection strategy.

`labels`  

The set of labels to consider.

## Discussion

The classifications and ground truth sequences are matched element by element in the order they are provided. Both sequences must have the same number of elements.

## See Also

### Creating the distribution

init(some Sequence&lt;(classification: ClassificationDistribution&lt;Label>, labels: Set&lt;Label>)>, strategy: MultiLabelClassificationMetrics&lt;Label>.ThresholdSelectionStrategy) throws

Creates multi-label classification metrics for classifications and ground truth labels.

init(some Sequence&lt;(classification: ClassificationDistribution&lt;Label>, labels: Set&lt;Label>)>, strategy: MultiLabelClassificationMetrics&lt;Label>.ThresholdSelectionStrategy, labels: Set&lt;Label>) throws

Creates multi-label classification metrics for classifications and ground truth labels.

init(classifications: some Sequence&lt;ClassificationDistribution&lt;Label>>, groundTruth: some Sequence&lt;Set&lt;Label>>, strategy: MultiLabelClassificationMetrics&lt;Label>.ThresholdSelectionStrategy) throws

Creates multi-label classification metrics for classifications and ground truth labels.

init(confidenceThresholds: [Label : Float])

Creates empty multi-label classification metrics.

enum ThresholdSelectionStrategy

A strategy for selecting a confidence threshold.

