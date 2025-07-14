

- Create ML Components
- ClassificationMetrics
-  init(predicted:groundTruth:labels:) 

Initializer

# init(predicted:groundTruth:labels:)

Creates classification metrics for predicted and ground truth labels.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
init(
    predicted: Predicted,
    groundTruth: Correct,
    labels: Set
) where Label == Predicted.Element, Predicted : Sequence, Correct : Sequence, Predicted.Element == Correct.Element
```

## Discussion

The predicted and ground truth collections are matched element by element in the order they are provided. Both collections must have the same number of elements. Labels not in the labels set are ignored.

- Parameters

  - predicted: The predicted labels.

  - groundTruth: The true labels.

  - labels: The set of labels to consider.

## See Also

### Creating the distribution

init&lt;Predicted, Correct>(Predicted, Correct)

Creates classification metrics for predicted and ground truth labels.

init()

Creates empty classification metrics.

init(some Sequence&lt;(predicted: Label, label: Label)>)

Creates classification metrics for a sequence of predicted and ground truth label pairs.

init&lt;S, Inner>(S) async throws

Creates classification metrics from a temporal sequence of annotated classifications.

init(some Sequence&lt;(predicted: Label, label: Label)>, labels: Set&lt;Label>)

Creates classification metrics for a sequence of predicted and ground truth label pairs.

