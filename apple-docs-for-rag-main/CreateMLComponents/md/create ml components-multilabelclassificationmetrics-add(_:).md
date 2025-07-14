

- Create ML Components
- MultiLabelClassificationMetrics
-  add(\_:) 

Instance Method

# add(\_:)

Updates the metrics with more pairs of classifications and ground truth labels.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
mutating func add(_ pairs: some Sequence, labels: Set)>)
```

Available when `Label` conforms to `Hashable`.

## Parameters 

`pairs`  

A sequence of classifications and true label pairs.

## See Also

### Updating the metrics

func add(classifications: some Sequence&lt;ClassificationDistribution&lt;Label>>, groundTruth: some Sequence&lt;Set&lt;Label>>)

Updates the metrics with more classifications and ground truth labels.

