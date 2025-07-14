

- Create ML Components
- MultiLabelClassificationMetrics
-  count(of:) 

Instance Method

# count(of:)

Returns the number of times a label appeared in the ground truth collection.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func count(of label: Label) -> Int
```

Available when `Label` conforms to `Hashable`.

## Parameters 

`label`  

The label.

## See Also

### Computing and scoring

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

func trueNegativeCount(of: Label) -> Int

Returns the number of times a label was not in the predicted or ground truth collections.

func truePositiveCount(of: Label) -> Int

Returns the number of times the predicted label matched the true label.

