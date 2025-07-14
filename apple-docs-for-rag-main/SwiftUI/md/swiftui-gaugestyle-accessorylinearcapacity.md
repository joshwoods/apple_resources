

- SwiftUI
- GaugeStyle
-  accessoryLinearCapacity 

Type Property

# accessoryLinearCapacity

A gauge style that displays bar that fills from leading to trailing edges as the gauge’s current value increases.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
static var accessoryLinearCapacity: AccessoryLinearCapacityGaugeStyle { get }
```

Available when `Self` is `AccessoryLinearCapacityGaugeStyle`.

## Discussion

Apply this style to a Gauge or to a view hierarchy that contains gauges using the gaugeStyle(_:) modifier:

```
Gauge(value: batteryLevel, in: 0...100) {
    Text("Battery Level")
}
.gaugeStyle(.accessoryLinearCapacity)
```

If you provide `minimumValueLabel` and `maximumValueLabel` parameters when you create the gauge, they appear on leading and trailing edges of the bar, respectively. The `label` appears above the gauge, and the `currentValueLabel` appears below.

## See Also

### Getting linear gauge styles

static var linear: LinearGaugeStyle

A gauge style that displays a bar with a marker that appears at a point along the bar to indicate the gauge’s current value.

static var linearCapacity: LinearCapacityGaugeStyle

A gauge style that displays a bar that fills from leading to trailing edges as the gauge’s current value increases.

static var accessoryLinear: AccessoryLinearGaugeStyle

A gauge style that displays bar with a marker that appears at a point along the bar to indicate the gauge’s current value.

