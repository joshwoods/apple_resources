

- Create ML Components
- ClassificationMetrics
-  init() 

Initializer

# init()

Creates empty classification metrics.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
init()
```

## See Also

### Creating the distribution

init&lt;Predicted, Correct>(Predicted, Correct)

Creates classification metrics for predicted and ground truth labels.

init(some Sequence&lt;(predicted: Label, label: Label)>)

Creates classification metrics for a sequence of predicted and ground truth label pairs.

init&lt;S, Inner>(S) async throws

Creates classification metrics from a temporal sequence of annotated classifications.

init(some Sequence&lt;(predicted: Label, label: Label)>, labels: Set&lt;Label>)

Creates classification metrics for a sequence of predicted and ground truth label pairs.

init&lt;Predicted, Correct>(predicted: Predicted, groundTruth: Correct, labels: Set&lt;Label>)

Creates classification metrics for predicted and ground truth labels.

