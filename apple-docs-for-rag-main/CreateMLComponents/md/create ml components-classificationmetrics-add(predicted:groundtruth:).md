

- Create ML Components
- ClassificationMetrics
-  add(predicted:groundTruth:) 

Instance Method

# add(predicted:groundTruth:)

Updates the metrics with more predicted and ground truth labels.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
mutating func add(
    predicted: some Sequence,
    groundTruth: some Sequence
)
```

## Parameters 

`predicted`  

The predicted labels.

`groundTruth`  

The true labels.

## Discussion

The predicted and ground truth sequences are matched element by element in the order they are provided. Both sequences must have the same number of elements.

## See Also

### Updating the metrics

func add(some Sequence&lt;(predicted: Label, label: Label)>)

Updates the metrics with more predicted and ground truth label pairs.

