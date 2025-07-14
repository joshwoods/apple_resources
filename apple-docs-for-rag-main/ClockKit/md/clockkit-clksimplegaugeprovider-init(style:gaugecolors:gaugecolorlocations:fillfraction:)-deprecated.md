

- ClockKit
- CLKSimpleGaugeProvider
-  init(style:gaugeColors:gaugeColorLocations:fillFraction:) Deprecated

Initializer

# init(style:gaugeColors:gaugeColorLocations:fillFraction:)

Creates a multicolor gauge.

watchOS 5.0–9.0Deprecated

``` source
convenience init(
    style: CLKGaugeProviderStyle,
    gaugeColors: [UIColor]?,
    gaugeColorLocations: [NSNumber]?,
    fillFraction: Float
)
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Parameters 

`style`  

The style defining the gauge’s visual appearance. For a list of valid styles, see CLKGaugeProviderStyle.

`gaugeColors`  

The gauge’s colors. These colors are displayed as a gradient.

`gaugeColorLocations`  

The location of each color along the gauge. Locations are values between `0.0` and `1.0`. If `nil`, the colors are evenly spaced along the gauge.

`fillFraction`  

The value displayed by the gauge. Use a value between `0.0` and `1.0`. For an empty gauge, use CLKSimpleGaugeProviderFillFractionEmpty.

## Return Value

A newly instantiated multicolor gauge.

## Discussion

If you provide both colors and locations, then the `gaugeColors` and `gaugeColorLocations` arrays must be the same length.

## See Also

### Creating a Simple Gauge Provider

convenience init(style: CLKGaugeProviderStyle, gaugeColor: UIColor, fillFraction: Float)

Creates a solid-color gauge.

Deprecated

