

- Create ML Components
- MultiLabelClassificationMetrics
-  MultiLabelClassificationMetrics.ThresholdSelectionStrategy 

Enumeration

# MultiLabelClassificationMetrics.ThresholdSelectionStrategy

A strategy for selecting a confidence threshold.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
enum ThresholdSelectionStrategy
```

Available when `Label` conforms to `Hashable`.

## Topics

### Selection strategies

case balancedPrecisionAndRecall

A confidence threshold strategy that balances precision and recall equivalently.

case fixed([Label : Float])

A confidence threshold strategy that uses the specified thresholds for each label.

case precision(Float, minimumRecall: Float)

A confidence threshold strategy for a specific precision that has at least a minimum recall value.

case recall(Float, minimumPrecision: Float)

A confidence threshold strategy for a recall precision that has at least a minimum precision value.

### Operators

static func == (MultiLabelClassificationMetrics&lt;Label>.ThresholdSelectionStrategy, MultiLabelClassificationMetrics&lt;Label>.ThresholdSelectionStrategy) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

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

init(confidenceThresholds: [Label : Float])

Creates empty multi-label classification metrics.

