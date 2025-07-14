

- ClockKit
- CLKComplicationTemplateGraphicCornerGaugeText
-  init(gaugeProvider:outerTextProvider:) Deprecated

Initializer

# init(gaugeProvider:outerTextProvider:)

Creates a template that has a gauge and an outer text element.

watchOS 7.0–9.0Deprecated

``` source
init(
    gaugeProvider: CLKGaugeProvider,
    outerTextProvider: CLKTextProvider
)
```

## Parameters 

`gaugeProvider`  

The gauge provider for the template.

`outerTextProvider`  

The text provider for the outer line of text. The template ignores this text provider’s tint color, and always displays the text with a system color.

## See Also

### Creating the Template

init(gaugeProvider: CLKGaugeProvider, leadingTextProvider: CLKTextProvider?, trailingTextProvider: CLKTextProvider?, outerTextProvider: CLKTextProvider)

Creates a template that has a gauge with leading and trailing text, and an outer text element.

Deprecated

