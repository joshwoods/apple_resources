

- Create ML Components
- MultiLabelClassificationMetrics
- MultiLabelClassificationMetrics.ThresholdSelectionStrategy
-  MultiLabelClassificationMetrics.ThresholdSelectionStrategy.balancedPrecisionAndRecall 

Case

# MultiLabelClassificationMetrics.ThresholdSelectionStrategy.balancedPrecisionAndRecall

A confidence threshold strategy that balances precision and recall equivalently.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
case balancedPrecisionAndRecall
```

## Discussion

Use this strategy to select a threshold for each label to maximize the f1-score.

## See Also

### Selection strategies

case fixed([Label : Float])

A confidence threshold strategy that uses the specified thresholds for each label.

case precision(Float, minimumRecall: Float)

A confidence threshold strategy for a specific precision that has at least a minimum recall value.

case recall(Float, minimumPrecision: Float)

A confidence threshold strategy for a recall precision that has at least a minimum precision value.

