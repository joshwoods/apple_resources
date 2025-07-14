

- Create ML Components
- ClassificationMetrics
-  init(\_:) 

Initializer

# init(\_:)

Creates classification metrics from a temporal sequence of annotated classifications.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
init(_ predicted: S) async throws where S : Sequence, Inner : TemporalSequence, S.Element == AnnotatedFeature, Inner.Feature == ClassificationDistribution
```

## Discussion

- Parameters

  - predicted: The predicted sequence of annotated temporal sequences of classification distributions.

## See Also

### Creating the distribution

init&lt;Predicted, Correct>(Predicted, Correct)

Creates classification metrics for predicted and ground truth labels.

init()

Creates empty classification metrics.

init(some Sequence&lt;(predicted: Label, label: Label)>)

Creates classification metrics for a sequence of predicted and ground truth label pairs.

init(some Sequence&lt;(predicted: Label, label: Label)>, labels: Set&lt;Label>)

Creates classification metrics for a sequence of predicted and ground truth label pairs.

init&lt;Predicted, Correct>(predicted: Predicted, groundTruth: Correct, labels: Set&lt;Label>)

Creates classification metrics for predicted and ground truth labels.

