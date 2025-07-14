

- SwiftUI
- GaugeStyle
-  linearCapacity 

Type Property

# linearCapacity

A gauge style that displays a bar that fills from leading to trailing edges as the gauge’s current value increases.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
static var linearCapacity: LinearCapacityGaugeStyle { get }
```

Available when `Self` is `LinearCapacityGaugeStyle`.

## Discussion

Apply this style to a Gauge or to a view hierarchy that contains gauges using the gaugeStyle(_:) modifier:

```
Gauge(value: batteryLevel, in: 0...100) {
    Text("Battery Level")
}
.gaugeStyle(.linearCapacity)
```

If you provide `minimumValueLabel` and `maximumValueLabel` parameters when you create the gauge, they appear on leading and trailing edges of the bar, respectively. The `label` appears above the gauge, and the `currentValueLabel` appears below.

## See Also

### Getting linear gauge styles

static var linear: LinearGaugeStyle

A gauge style that displays a bar with a marker that appears at a point along the bar to indicate the gauge’s current value.

static var accessoryLinear: AccessoryLinearGaugeStyle

A gauge style that displays bar with a marker that appears at a point along the bar to indicate the gauge’s current value.

static var accessoryLinearCapacity: AccessoryLinearCapacityGaugeStyle

A gauge style that displays bar that fills from leading to trailing edges as the gauge’s current value increases.

