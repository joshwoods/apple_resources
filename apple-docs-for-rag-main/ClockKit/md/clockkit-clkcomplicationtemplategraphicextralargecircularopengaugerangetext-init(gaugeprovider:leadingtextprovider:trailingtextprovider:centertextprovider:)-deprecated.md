

- ClockKit
- CLKComplicationTemplateGraphicExtraLargeCircularOpenGaugeRangeText
-  init(gaugeProvider:leadingTextProvider:trailingTextProvider:centerTextProvider:) Deprecated

Initializer

# init(gaugeProvider:leadingTextProvider:trailingTextProvider:centerTextProvider:)

Creates a new template that has an open, circular gauge with leading and trailing text, and a central text element.

watchOS 7.0–9.0Deprecated

``` source
init(
    gaugeProvider: CLKGaugeProvider,
    leadingTextProvider: CLKTextProvider,
    trailingTextProvider: CLKTextProvider,
    centerTextProvider: CLKTextProvider
)
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Parameters 

`gaugeProvider`  

The gauge provider for the template.

`leadingTextProvider`  

The text provider for the leading text. The template supports multicolored text from this text provider.

`trailingTextProvider`  

The text provider for the trailing text. The template supports multicolored text from this text provider.

`centerTextProvider`  

The text provider for the center text. The template supports multicolored text from this text provider.

