

- SwiftUI
- Gauge
-  init(value:in:label:currentValueLabel:minimumValueLabel:maximumValueLabel:markedValueLabels:) 

Initializer

# init(value:in:label:currentValueLabel:minimumValueLabel:maximumValueLabel:markedValueLabels:)

Creates a gauge representing a value within a range.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
init(
    value: V,
    in bounds: ClosedRange = 0...1,
    @ViewBuilder label: () -> Label,
    @ViewBuilder currentValueLabel: () -> CurrentValueLabel,
    @ViewBuilder minimumValueLabel: () -> BoundsLabel,
    @ViewBuilder maximumValueLabel: () -> BoundsLabel,
    @ViewBuilder markedValueLabels: () -> MarkedValueLabels
) where V : BinaryFloatingPoint
```

## Parameters 

`value`  

The value to show in the gauge.

`bounds`  

The range of the valid values. Defaults to `0...1`.

`label`  

A view that describes the purpose of the gauge.

`currentValueLabel`  

A view that describes the current value of the gauge.

`minimumValueLabel`  

A view that describes the lower bounds of the gauge.

`maximumValueLabel`  

A view that describes the upper bounds of the gauge.

`markedValueLabels`  

A view builder containing tagged views. each of which describes a particular value of the gauge. The method ignores this parameter.

## See Also

### Creating a gauge

init&lt;V>(value: V, in: ClosedRange&lt;V>, label: () -> Label)

Creates a gauge showing a value within a range and describes the gauge’s purpose and current value.

init&lt;V>(value: V, in: ClosedRange&lt;V>, label: () -> Label, currentValueLabel: () -> CurrentValueLabel)

Creates a gauge showing a value within a range and that describes the gauge’s purpose and current value.

init&lt;V>(value: V, in: ClosedRange&lt;V>, label: () -> Label, currentValueLabel: () -> CurrentValueLabel, markedValueLabels: () -> MarkedValueLabels)

Creates a gauge representing a value within a range.

init&lt;V>(value: V, in: ClosedRange&lt;V>, label: () -> Label, currentValueLabel: () -> CurrentValueLabel, minimumValueLabel: () -> BoundsLabel, maximumValueLabel: () -> BoundsLabel)

Creates a gauge showing a value within a range and describes the gauge’s current, minimum, and maximum values.

