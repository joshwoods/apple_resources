

- ClockKit
- CLKComplicationTemplateGraphicExtraLargeCircularOpenGaugeSimpleText
-  init(gaugeProvider:bottomTextProvider:centerTextProvider:) Deprecated

Initializer

# init(gaugeProvider:bottomTextProvider:centerTextProvider:)

Creates a new template with an open circular gauge, a small text element at the bottom, and a larger text element in the center.

watchOS 7.0–9.0Deprecated

``` source
init(
    gaugeProvider: CLKGaugeProvider,
    bottomTextProvider: CLKTextProvider,
    centerTextProvider: CLKTextProvider
)
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Parameters 

`gaugeProvider`  

The gauge provider for the template.

`bottomTextProvider`  

The text provider for the bottom text. The template supports multicolored text from this text provider.

`centerTextProvider`  

The text provider for the center text. The template supports multicolored text from this text provider.

