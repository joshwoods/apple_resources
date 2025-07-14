

- Create ML Components
- MultiLabelClassificationMetrics
-  trueNegativeCount(of:) 

Instance Method

# trueNegativeCount(of:)

Returns the number of times a label was not in the predicted or ground truth collections.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func trueNegativeCount(of label: Label) -> Int
```

Available when `Label` conforms to `Hashable`.

## Parameters 

`label`  

The label to use as true positive.

## Return Value

The true negative count.

## Discussion

If the label does not have a confidence threshold, the true negative count is 0. If the label has a confidence threshold NaN, the true negative count is the number elements in the ground truth collection that do not contain the label. If the label is not in the known set of labels, the true negative count is 0.

## See Also

### Computing and scoring

func count(of: Label) -> Int

Returns the number of times a label appeared in the ground truth collection.

func f1Score(for: Label) -> Float

Computes the F1 score from predicted and ground truth values.

func falseNegativeCount(of: Label) -> Int

Returns the number of times a true label was not predicted.

func falsePositiveCount(of: Label) -> Int

Returns the number of times the predicted label did not match the true label.

func precisionScore(for: Label) -> Float

Computes the precision score for a class label.

func recallScore(for: Label) -> Float

Computes the recall score for a class label.

func truePositiveCount(of: Label) -> Int

Returns the number of times the predicted label matched the true label.

