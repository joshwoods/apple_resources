

- Create ML Components
- MultiLabelClassificationMetrics
-  init(\_:strategy:) 

Initializer

# init(\_:strategy:)

Creates multi-label classification metrics for classifications and ground truth labels.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
init(
    _ pairs: some Sequence, labels: Set)>,
    strategy: MultiLabelClassificationMetrics.ThresholdSelectionStrategy
) throws
```

## Parameters 

`pairs`  

A sequence of classifications and true label pairs.

`strategy`  

A label confidence threshold selection strategy.

## See Also

### Creating the distribution

init(some Sequence&lt;(classification: ClassificationDistribution&lt;Label>, labels: Set&lt;Label>)>, strategy: MultiLabelClassificationMetrics&lt;Label>.ThresholdSelectionStrategy, labels: Set&lt;Label>) throws

Creates multi-label classification metrics for classifications and ground truth labels.

init(classifications: some Sequence&lt;ClassificationDistribution&lt;Label>>, groundTruth: some Sequence&lt;Set&lt;Label>>, strategy: MultiLabelClassificationMetrics&lt;Label>.ThresholdSelectionStrategy) throws

Creates multi-label classification metrics for classifications and ground truth labels.

init(classifications: some Sequence&lt;ClassificationDistribution&lt;Label>>, groundTruth: some Sequence&lt;Set&lt;Label>>, strategy: MultiLabelClassificationMetrics&lt;Label>.ThresholdSelectionStrategy, labels: Set&lt;Label>) throws

Creates multi-label classification metrics for classifications and ground truth labels.

init(confidenceThresholds: [Label : Float])

Creates empty multi-label classification metrics.

enum ThresholdSelectionStrategy

A strategy for selecting a confidence threshold.

