

- ClockKit
- CLKSimpleGaugeProvider
-  init(style:gaugeColor:fillFraction:) Deprecated

Initializer

# init(style:gaugeColor:fillFraction:)

Creates a solid-color gauge.

watchOS 5.0–9.0Deprecated

``` source
convenience init(
    style: CLKGaugeProviderStyle,
    gaugeColor color: UIColor,
    fillFraction: Float
)
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Parameters 

`style`  

The style defining the gauge’s visual appearance. For a list of valid styles, see CLKGaugeProviderStyle.

`color`  

The gauge’s color.

`fillFraction`  

The value displayed by the gauge. Use a value between `0.0` and `1.0`. For an empty gauge, use CLKSimpleGaugeProviderFillFractionEmpty.

## Return Value

A newly instantiated solid-color gauge.

## See Also

### Creating a Simple Gauge Provider

convenience init(style: CLKGaugeProviderStyle, gaugeColors: [UIColor]?, gaugeColorLocations: [NSNumber]?, fillFraction: Float)

Creates a multicolor gauge.

Deprecated

