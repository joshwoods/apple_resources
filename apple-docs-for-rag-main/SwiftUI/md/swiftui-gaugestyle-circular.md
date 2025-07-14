

- SwiftUI
- GaugeStyle
-  circular 

Type Property

# circular

A gauge style that displays an open ring with a marker that appears at a point along the ring to indicate the gauge’s current value.

watchOS 7.0+

``` source
@MainActor @preconcurrency
static var circular: CircularGaugeStyle { get }
```

Available when `Self` is `CircularGaugeStyle`.

## Discussion

Apply this style to a Gauge or to a view hierarchy that contains gauges using the gaugeStyle(_:) modifier:

```
Gauge(value: batteryLevel, in: 0...100) {
    Text("Battery Level")
}
.gaugeStyle(.circular)
```

This style displays the gauge’s `currentValueLabel` value at the center of the gauge. If you provide `minimumValueLabel` and `maximumValueLabel` parameters when you create the gauge, they appear in the opening at the bottom of the ring. Otherwise, the gauge places its label in that location.

## See Also

### Getting circular gauge styles

static var accessoryCircular: AccessoryCircularGaugeStyle

A gauge style that displays an open ring with a marker that appears at a point along the ring to indicate the gauge’s current value.

static var accessoryCircularCapacity: AccessoryCircularCapacityGaugeStyle

A gauge style that displays a closed ring that’s partially filled in to indicate the gauge’s current value.

