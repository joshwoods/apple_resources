

- SwiftUI
- Gauge
-  init(value:in:label:currentValueLabel:) 

Initializer

# init(value:in:label:currentValueLabel:)

Creates a gauge showing a value within a range and that describes the gauge’s purpose and current value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
init(
    value: V,
    in bounds: ClosedRange = 0...1,
    @ViewBuilder label: () -> Label,
    @ViewBuilder currentValueLabel: () -> CurrentValueLabel
) where BoundsLabel == EmptyView, MarkedValueLabels == EmptyView, V : BinaryFloatingPoint
```

## Parameters 

`value`  

The value to show on the gauge.

`bounds`  

The range of the valid values. Defaults to `0...1`.

`label`  

A view that describes the purpose of the gauge.

`currentValueLabel`  

A view that describes the current value of the gauge.

## Discussion

Use this method to create a gauge that displays a value within a range you supply with labels that describe the purpose of the gauge and its current value. In the example below, a gauge using the circular style shows its current value of `67` along with a label describing the (BPM) for the gauge:

```
struct SimpleGauge: View {
    @State private var current = 67.0

    var body: some View {
        Gauge(value: currrent, in: 0...170) {
            Text("BPM")
        } currentValueLabel: {
            Text("\(current)")
        }
        .gaugeStyle(.circular)
   }
}
```

## See Also

### Creating a gauge

init&lt;V>(value: V, in: ClosedRange&lt;V>, label: () -> Label)

Creates a gauge showing a value within a range and describes the gauge’s purpose and current value.

init&lt;V>(value: V, in: ClosedRange&lt;V>, label: () -> Label, currentValueLabel: () -> CurrentValueLabel, markedValueLabels: () -> MarkedValueLabels)

Creates a gauge representing a value within a range.

init&lt;V>(value: V, in: ClosedRange&lt;V>, label: () -> Label, currentValueLabel: () -> CurrentValueLabel, minimumValueLabel: () -> BoundsLabel, maximumValueLabel: () -> BoundsLabel)

Creates a gauge showing a value within a range and describes the gauge’s current, minimum, and maximum values.

init&lt;V>(value: V, in: ClosedRange&lt;V>, label: () -> Label, currentValueLabel: () -> CurrentValueLabel, minimumValueLabel: () -> BoundsLabel, maximumValueLabel: () -> BoundsLabel, markedValueLabels: () -> MarkedValueLabels)

Creates a gauge representing a value within a range.

