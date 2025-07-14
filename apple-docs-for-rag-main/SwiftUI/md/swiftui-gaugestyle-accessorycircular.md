

- SwiftUI
- GaugeStyle
-  accessoryCircular 

Type Property

# accessoryCircular

A gauge style that displays an open ring with a marker that appears at a point along the ring to indicate the gauge’s current value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
static var accessoryCircular: AccessoryCircularGaugeStyle { get }
```

Available when `Self` is `AccessoryCircularGaugeStyle`.

## Discussion

Apply this style to a Gauge or to a view hierarchy that contains gauges using the gaugeStyle(_:) modifier:

```
Gauge(value: batteryLevel, in: 0...100) {
    Text("Battery Level")
}
.gaugeStyle(.accessoryCircular)
```

This style displays the gauge’s `currentValueLabel` value at the center of the gauge. If you provide `minimumValueLabel` and `maximumValueLabel` parameters when you create the gauge, they appear in the opening at the bottom of the ring. Otherwise, the gauge places its label in that location.

## See Also

### Getting circular gauge styles

static var circular: CircularGaugeStyle

A gauge style that displays an open ring with a marker that appears at a point along the ring to indicate the gauge’s current value.

static var accessoryCircularCapacity: AccessoryCircularCapacityGaugeStyle

A gauge style that displays a closed ring that’s partially filled in to indicate the gauge’s current value.

