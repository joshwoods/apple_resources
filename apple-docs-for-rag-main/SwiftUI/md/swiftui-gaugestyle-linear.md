

- SwiftUI
- GaugeStyle
-  linear 

Type Property

# linear

A gauge style that displays a bar with a marker that appears at a point along the bar to indicate the gauge’s current value.

watchOS 7.0+

``` source
@MainActor @preconcurrency
static var linear: LinearGaugeStyle { get }
```

Available when `Self` is `LinearGaugeStyle`.

## Discussion

Apply this style to a Gauge or to a view hierarchy that contains gauges using the gaugeStyle(_:) modifier:

```
Gauge(value: batteryLevel, in: 0...100) {
    Text("Battery Level")
}
.gaugeStyle(.linear)
```

If you provide `minimumValueLabel` and `maximumValueLabel` parameters when you create the gauge, they appear on leading and trailing edges of the bar, respectively. Otherwise, the gauge displays the `currentValueLabel` value on the leading edge.

## See Also

### Getting linear gauge styles

static var linearCapacity: LinearCapacityGaugeStyle

A gauge style that displays a bar that fills from leading to trailing edges as the gauge’s current value increases.

static var accessoryLinear: AccessoryLinearGaugeStyle

A gauge style that displays bar with a marker that appears at a point along the bar to indicate the gauge’s current value.

static var accessoryLinearCapacity: AccessoryLinearCapacityGaugeStyle

A gauge style that displays bar that fills from leading to trailing edges as the gauge’s current value increases.

