

- SwiftUI
- Gauge
-  init(value:in:label:) 

Initializer

# init(value:in:label:)

Creates a gauge showing a value within a range and describes the gauge’s purpose and current value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
init(
    value: V,
    in bounds: ClosedRange = 0...1,
    @ViewBuilder label: () -> Label
) where CurrentValueLabel == EmptyView, BoundsLabel == EmptyView, MarkedValueLabels == EmptyView, V : BinaryFloatingPoint
```

## Parameters 

`value`  

The value to show in the gauge.

`bounds`  

The range of the valid values. Defaults to `0...1`.

`label`  

A view that describes the purpose of the gauge.

## Discussion

Use this modifier to create a gauge that shows the value at its relative position along the gauge and a label describing the gauge’s purpose. In the example below, the gauge has a range of `0...1`, the indicator is set to `0.4`, or 40 percent of the distance along the gauge:

```
struct SimpleGauge: View {
    @State private var batteryLevel = 0.4

    var body: some View {
        Gauge(value: batteryLevel) {
            Text("Battery Level")
        }
    }
}
```

## See Also

### Creating a gauge

init&lt;V>(value: V, in: ClosedRange&lt;V>, label: () -> Label, currentValueLabel: () -> CurrentValueLabel)

Creates a gauge showing a value within a range and that describes the gauge’s purpose and current value.

init&lt;V>(value: V, in: ClosedRange&lt;V>, label: () -> Label, currentValueLabel: () -> CurrentValueLabel, markedValueLabels: () -> MarkedValueLabels)

Creates a gauge representing a value within a range.

init&lt;V>(value: V, in: ClosedRange&lt;V>, label: () -> Label, currentValueLabel: () -> CurrentValueLabel, minimumValueLabel: () -> BoundsLabel, maximumValueLabel: () -> BoundsLabel)

Creates a gauge showing a value within a range and describes the gauge’s current, minimum, and maximum values.

init&lt;V>(value: V, in: ClosedRange&lt;V>, label: () -> Label, currentValueLabel: () -> CurrentValueLabel, minimumValueLabel: () -> BoundsLabel, maximumValueLabel: () -> BoundsLabel, markedValueLabels: () -> MarkedValueLabels)

Creates a gauge representing a value within a range.

