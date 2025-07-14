

- Create ML Components
- ClassificationMetrics
-  precisionScore(label:) 

Instance Method

# precisionScore(label:)

Computes the precision score for a class label.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func precisionScore(label: Label) -> Double
```

Available when `Label` conforms to `Hashable`.

## Parameters 

`label`  

The label to use as true positive.

## Return Value

The precision score for the given label.

## Discussion

Precision score is computed as the ratio `tp / (tp + fp)` where `tp` is the number of true positives and `fp` is the number of false positives.

## See Also

### Computing and scoring

func makeConfusionMatrix() -> MLShapedArray&lt;Float>

Computes the confusion matrix.

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

func truePositiveCount(of: Label) -> Int

Returns the number of times the predicted label matched the true label.

func falseNegativeCount(of: Label) -> Int

Returns the number of times a true label was not predicted.

func falsePositiveCount(of: Label) -> Int

Returns the number of times the predicted label did not match the true label.

func f1Score(label: Label) -> Double

Computes the F1 score for a class label.

func mapLabels&lt;T>((Label) throws -> T) rethrows -> ClassificationMetrics&lt;T>

Returns new classification metrics where the labels are the result of applying a transformation.

