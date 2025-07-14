

- ClockKit
- CLKComplicationTemplateGraphicRectangularTextGauge
-  init(headerImageProvider:headerTextProvider:body1TextProvider:gaugeProvider:) Deprecated

Initializer

# init(headerImageProvider:headerTextProvider:body1TextProvider:gaugeProvider:)

Creates a new template that has a header row with an image and text, body text, and a gauge.

watchOS 7.0–9.0Deprecated

``` source
init(
    headerImageProvider: CLKFullColorImageProvider?,
    headerTextProvider: CLKTextProvider,
    body1TextProvider: CLKTextProvider,
    gaugeProvider: CLKGaugeProvider
)
```

## Parameters 

`headerImageProvider`  

A full-color image provider.

`headerTextProvider`  

The text provider for the header text. The template supports multicolored text from this text provider.

`body1TextProvider`  

The text provider for the body text. The template supports multicolored text from this text provider.

`gaugeProvider`  

The gauge provider for the template.

## See Also

### Creating the Template

init(headerTextProvider: CLKTextProvider, body1TextProvider: CLKTextProvider, gaugeProvider: CLKGaugeProvider)

Creates a new template that has header text, body text, and a gauge.

Deprecated

