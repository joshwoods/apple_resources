

- ClockKit
- CLKTimeIntervalGaugeProvider
-  init(style:gaugeColors:gaugeColorLocations:start:end:) Deprecated

Initializer

# init(style:gaugeColors:gaugeColorLocations:start:end:)

Creates a time interval gauge that fills as time passes.

watchOS 5.0–9.0Deprecated

``` source
convenience init(
    style: CLKGaugeProviderStyle,
    gaugeColors: [UIColor]?,
    gaugeColorLocations: [NSNumber]?,
    start startDate: Date,
    end endDate: Date
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

`startDate`  

The start time and date.

`endDate`  

The end time and date. This value must be later than or equal to the start date.

## Return Value

A newly instantiated time interval gauge provider.

## Discussion

The gauge shows the amount of time that has elapsed, based on the current time relative to the specified start and end dates. The gauge fills as it counts up from the start time to the end time.

If you provide both colors and locations, then the `gaugeColors` and `gaugeColorLocations` arrays must be the same length.

## See Also

### Creating a Time Interval Gauge

convenience init(style: CLKGaugeProviderStyle, gaugeColors: [UIColor]?, gaugeColorLocations: [NSNumber]?, start: Date, startFillFraction: Float, end: Date, endFillFraction: Float)

Creates a time interval gauge, letting you specify whether the gauge fills or empties as time passes.

Deprecated

