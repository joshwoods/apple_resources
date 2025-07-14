

- Create ML Components
- MultiLabelClassificationMetrics
- MultiLabelClassificationMetrics.ThresholdSelectionStrategy
-  MultiLabelClassificationMetrics.ThresholdSelectionStrategy.fixed(\_:) 

Case

# MultiLabelClassificationMetrics.ThresholdSelectionStrategy.fixed(\_:)

A confidence threshold strategy that uses the specified thresholds for each label.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
case fixed([Label : Float])
```

## See Also

### Selection strategies

case balancedPrecisionAndRecall

A confidence threshold strategy that balances precision and recall equivalently.

case precision(Float, minimumRecall: Float)

A confidence threshold strategy for a specific precision that has at least a minimum recall value.

case recall(Float, minimumPrecision: Float)

A confidence threshold strategy for a recall precision that has at least a minimum precision value.

