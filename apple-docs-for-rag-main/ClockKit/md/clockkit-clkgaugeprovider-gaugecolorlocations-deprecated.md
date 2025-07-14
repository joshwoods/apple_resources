

- ClockKit
- CLKGaugeProvider
-  gaugeColorLocations Deprecated

Instance Property

# gaugeColorLocations

The location of each color in a multicolor gauge’s gradient.

watchOS 5.0–9.0Deprecated

``` source
var gaugeColorLocations: [NSNumber]? { get }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

This property specifies the location of each color in the gaugeColors array. Each location must be a value between `0.0` and `1.0`.

A gauge with more than one color appears as a gradient. The provider specifies the colors using the gaugeColors property. The gaugeColors and gaugeColorLocations properties must have the same number of elements.

## See Also

### Setting the Gauge’s Appearance

var gaugeColors: [UIColor]?

The colors of the gauge.

Deprecated

var style: CLKGaugeProviderStyle

The style that defines the gauge’s appearance.

Deprecated

