

- Create ML Components
- ClassificationMetrics
-  add(\_:) 

Instance Method

# add(\_:)

Updates the metrics with more predicted and ground truth label pairs.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
mutating func add(_ pairs: some Sequence)
```

## Parameters 

`pairs`  

A collection of predicted and true label pairs.

## See Also

### Updating the metrics

func add(predicted: some Sequence&lt;Label>, groundTruth: some Sequence&lt;Label>)

Updates the metrics with more predicted and ground truth labels.

