

- Create ML Components
- ClassificationMetrics
-  truePositiveCount(of:) 

Instance Method

# truePositiveCount(of:)

Returns the number of times the predicted label matched the true label.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func truePositiveCount(of label: Label) -> Int
```

## Parameters 

`label`  

A label.

## See Also

### Computing and scoring

func makeConfusionMatrix() -> MLShapedArray&lt;Float>

Computes the confusion matrix.

func precisionScore(label: Label) -> Double

Computes the precision score for a class label.

func recallScore(label: Label) -> Double

Computes the recall score for a class label.

func count(label: Label) -> Int

Returns the number of times a label appeared in the ground truth collection.

func count(predicted: Label) -> Int

Returns the number of times a label appeared in the predicted collection.

func count(predicted: Label, label: Label) -> Int

Returns the number of times a predicted, true label pair appeared in the label collections.

func trueNegativeCount(of: Label) -> Int

Returns the number of times a label was not in the predicted or ground truth collections.

func falseNegativeCount(of: Label) -> Int

Returns the number of times a true label was not predicted.

func falsePositiveCount(of: Label) -> Int

Returns the number of times the predicted label did not match the true label.

func f1Score(label: Label) -> Double

Computes the F1 score for a class label.

func mapLabels&lt;T>((Label) throws -> T) rethrows -> ClassificationMetrics&lt;T>

Returns new classification metrics where the labels are the result of applying a transformation.

