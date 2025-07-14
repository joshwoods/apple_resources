

- Create ML Components
- ClassificationMetrics
-  makeConfusionMatrix() 

Instance Method

# makeConfusionMatrix()

Computes the confusion matrix.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func makeConfusionMatrix() -> MLShapedArray where Label : Comparable, Label : Decodable, Label : Encodable
```

## Discussion

The `i`th row and `j`th column value indicate the count of true label being the `i`th class and predicted label being the `j`th class. The labels are sorted in ascending order.

## See Also

### Computing and scoring

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

