

- Create ML Components
- ClassificationMetrics
-  init(\_:\_:) 

Initializer

# init(\_:\_:)

Creates classification metrics for predicted and ground truth labels.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
init(
    _ predicted: Predicted,
    _ groundTruth: Correct
) where Label == Predicted.Element, Predicted : Collection, Correct : Collection, Predicted.Element == Correct.Element
```

## Discussion

The predicted and ground truth collections are matched element by element in the order they are provided. Both collections must have the same number of elements.

- Parameters

  - predicted: The predicted labels.

  - groundTruth: The true labels.

## See Also

### Creating the distribution

init()

Creates empty classification metrics.

init(some Sequence&lt;(predicted: Label, label: Label)>)

Creates classification metrics for a sequence of predicted and ground truth label pairs.

init&lt;S, Inner>(S) async throws

Creates classification metrics from a temporal sequence of annotated classifications.

init(some Sequence&lt;(predicted: Label, label: Label)>, labels: Set&lt;Label>)

Creates classification metrics for a sequence of predicted and ground truth label pairs.

init&lt;Predicted, Correct>(predicted: Predicted, groundTruth: Correct, labels: Set&lt;Label>)

Creates classification metrics for predicted and ground truth labels.

