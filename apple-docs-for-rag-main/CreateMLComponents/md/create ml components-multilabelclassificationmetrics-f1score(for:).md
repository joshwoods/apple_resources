

- Create ML Components
- MultiLabelClassificationMetrics
-  f1Score(for:) 

Instance Method

# f1Score(for:)

Computes the F1 score from predicted and ground truth values.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func f1Score(for label: Label) -> Float
```

Available when `Label` conforms to `Hashable`.

## Parameters 

`label`  

The label to use as true positive.

## Return Value

The F1 score for the given label.

## Discussion

The balanced F-score, or F1 score, is computed as the harmonic mean of the precision and recall. If the provided label does not have a confidence threshold, the F1 score is NaN.

## See Also

### Computing and scoring

func count(of: Label) -> Int

Returns the number of times a label appeared in the ground truth collection.

func falseNegativeCount(of: Label) -> Int

Returns the number of times a true label was not predicted.

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

