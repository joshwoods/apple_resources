

- Create ML Components
- MultiLabelClassificationMetrics
-  falseNegativeCount(of:) 

Instance Method

# falseNegativeCount(of:)

Returns the number of times a true label was not predicted.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func falseNegativeCount(of label: Label) -> Int
```

Available when `Label` conforms to `Hashable`.

## Parameters 

`label`  

The label to use as true positive.

## Return Value

The false negative count.

## Discussion

If the label does not have a confidence threshold, the false negative count is 0. If the label has a confidence threshold NaN, the false negative count is the number of elements in the ground truth labels collection that do not contain the label. If the label is not in the known set of labels, the false negative count is 0.

## See Also

### Computing and scoring

func count(of: Label) -> Int

Returns the number of times a label appeared in the ground truth collection.

func f1Score(for: Label) -> Float

Computes the F1 score from predicted and ground truth values.

func falsePositiveCount(of: Label) -> Int

Returns the number of times the predicted label did not match the true label.

func precisionScore(for: Label) -> Float

Computes the precision score for a class label.

func recallScore(for: Label) -> Float

Computes the recall score for a class label.

func trueNegativeCount(of: Label) -> Int

Returns the number of times a label was not in the predicted or ground truth collections.

func truePositiveCount(of: Label) -> Int

Returns the number of times the predicted label matched the true label.

