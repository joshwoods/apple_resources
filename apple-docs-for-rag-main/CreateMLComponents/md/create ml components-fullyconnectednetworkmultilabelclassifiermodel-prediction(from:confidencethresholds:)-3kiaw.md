

- Create ML Components
- FullyConnectedNetworkMultiLabelClassifierModel
-  prediction(from:confidenceThresholds:) 

Instance Method

# prediction(from:confidenceThresholds:)

Performs a sequence of predictions and keeps label-confidence pairs that are greater than or equal to the provided confidence thresholds.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func prediction(
    from input: S,
    confidenceThresholds: [Label : Scalar]
) throws -> [ClassificationDistribution] where S : Sequence, S.Element == MLShapedArray
```

## Parameters 

`input`  

A sequence of model inputs.

`confidenceThresholds`  

A dictionary of label and confidence threshold pairs.

## Return Value

An array of classification distributions.

## Discussion

When the confidence threshold is `NaN`, the label-confidence pair is not included in the result, regardless of the label’s confidence.

## See Also

### Performing a prediction

func prediction(from: FullyConnectedNetworkMultiLabelClassifierModel&lt;Scalar, Label>.Input, confidenceThresholds: [Label : Scalar]) throws -> ClassificationDistribution&lt;Label>

Performs a prediction and keeps label-confidence pairs that are greater than or equal to the provided confidence thresholds.

