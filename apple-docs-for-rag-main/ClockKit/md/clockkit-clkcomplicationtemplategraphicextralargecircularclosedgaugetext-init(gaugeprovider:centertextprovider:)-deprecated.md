

- ClockKit
- CLKComplicationTemplateGraphicExtraLargeCircularClosedGaugeText
-  init(gaugeProvider:centerTextProvider:) Deprecated

Initializer

# init(gaugeProvider:centerTextProvider:)

Creates a new template with a closed circular gauge with text in the center.

watchOS 7.0–9.0Deprecated

``` source
init(
    gaugeProvider: CLKGaugeProvider,
    centerTextProvider: CLKTextProvider
)
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Parameters 

`gaugeProvider`  

The gauge provider for the template.

`centerTextProvider`  

The text provider for the center text. The template supports multicolored text from this text provider.

