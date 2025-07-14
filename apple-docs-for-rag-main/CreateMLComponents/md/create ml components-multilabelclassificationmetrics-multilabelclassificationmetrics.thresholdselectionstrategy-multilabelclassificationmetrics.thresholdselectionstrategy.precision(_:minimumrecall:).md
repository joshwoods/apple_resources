

- Create ML Components
- MultiLabelClassificationMetrics
- MultiLabelClassificationMetrics.ThresholdSelectionStrategy
-  MultiLabelClassificationMetrics.ThresholdSelectionStrategy.precision(\_:minimumRecall:) 

Case

# MultiLabelClassificationMetrics.ThresholdSelectionStrategy.precision(\_:minimumRecall:)

A confidence threshold strategy for a specific precision that has at least a minimum recall value.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
case precision(
    Float,
    minimumRecall: Float
)
```

## Discussion

This strategy selects a threshold for each label by searching for the specified precision value on the label’s precision-recall curve. At the precision, the recall must be greater than or equal to the minimum recall value, otherwise a NaN threshold for the corresponding label is returned.

Use this strategy to reduce the rate of false-positive predictions while constraining the false-negative predictions.

## See Also

### Selection strategies

case balancedPrecisionAndRecall

A confidence threshold strategy that balances precision and recall equivalently.

case fixed([Label : Float])

A confidence threshold strategy that uses the specified thresholds for each label.

case recall(Float, minimumPrecision: Float)

A confidence threshold strategy for a recall precision that has at least a minimum precision value.

