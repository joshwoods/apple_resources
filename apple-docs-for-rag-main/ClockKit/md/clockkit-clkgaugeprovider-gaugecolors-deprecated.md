

- ClockKit
- CLKGaugeProvider
-  gaugeColors Deprecated

Instance Property

# gaugeColors

The colors of the gauge.

watchOS 5.0–9.0Deprecated

``` source
var gaugeColors: [UIColor]? { get }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

A gauge with more than one color appears as a gradient. The provider specifies the location of the colors using the gaugeColorLocations property. The gaugeColors and gaugeColorLocations properties must have the same number of elements.

Note

Tinted graphic complications display gauges using a solid color chosen by the user. The gauge colors have no affect on the appearance of these complications.

## See Also

### Setting the Gauge’s Appearance

var gaugeColorLocations: [NSNumber]?

The location of each color in a multicolor gauge’s gradient.

Deprecated

var style: CLKGaugeProviderStyle

The style that defines the gauge’s appearance.

Deprecated

