

- Create ML Components
- MultiLabelClassificationMetrics
-  add(classifications:groundTruth:) 

Instance Method

# add(classifications:groundTruth:)

Updates the metrics with more classifications and ground truth labels.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
mutating func add(
    classifications: some Sequence>,
    groundTruth: some Sequence>
)
```

Available when `Label` conforms to `Hashable`.

## Parameters 

`classifications`  

A collection of classifications.

`groundTruth`  

A collection of true labels.

## Discussion

The classifications and ground truth sequences are matched element by element in the order they are provided. Both sequences must have the same number of elements.

## See Also

### Updating the metrics

func add(some Sequence&lt;(classification: ClassificationDistribution&lt;Label>, labels: Set&lt;Label>)>)

Updates the metrics with more pairs of classifications and ground truth labels.

