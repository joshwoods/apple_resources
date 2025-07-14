

- Create ML Components
- MultiLabelClassificationMetrics
-  init(confidenceThresholds:) 

Initializer

# init(confidenceThresholds:)

Creates empty multi-label classification metrics.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
init(confidenceThresholds: [Label : Float])
```

Available when `Label` conforms to `Hashable`.

## Parameters 

`confidenceThresholds`  

A dictionary of label and confidence thresholds.

## See Also

### Creating the distribution

init(some Sequence&lt;(classification: ClassificationDistribution&lt;Label>, labels: Set&lt;Label>)>, strategy: MultiLabelClassificationMetrics&lt;Label>.ThresholdSelectionStrategy) throws

Creates multi-label classification metrics for classifications and ground truth labels.

init(some Sequence&lt;(classification: ClassificationDistribution&lt;Label>, labels: Set&lt;Label>)>, strategy: MultiLabelClassificationMetrics&lt;Label>.ThresholdSelectionStrategy, labels: Set&lt;Label>) throws

Creates multi-label classification metrics for classifications and ground truth labels.

init(classifications: some Sequence&lt;ClassificationDistribution&lt;Label>>, groundTruth: some Sequence&lt;Set&lt;Label>>, strategy: MultiLabelClassificationMetrics&lt;Label>.ThresholdSelectionStrategy) throws

Creates multi-label classification metrics for classifications and ground truth labels.

init(classifications: some Sequence&lt;ClassificationDistribution&lt;Label>>, groundTruth: some Sequence&lt;Set&lt;Label>>, strategy: MultiLabelClassificationMetrics&lt;Label>.ThresholdSelectionStrategy, labels: Set&lt;Label>) throws

Creates multi-label classification metrics for classifications and ground truth labels.

enum ThresholdSelectionStrategy

A strategy for selecting a confidence threshold.

