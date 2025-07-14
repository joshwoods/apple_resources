

- ClockKit
- CLKComplicationTemplateGraphicCircularOpenGaugeImage
-  init(gaugeProvider:bottomImageProvider:centerTextProvider:) Deprecated

Initializer

# init(gaugeProvider:bottomImageProvider:centerTextProvider:)

Creates a new template that has an open circular gauge, a small image at the bottom, and a small amount of text in the center.

watchOS 7.0–9.0Deprecated

``` source
init(
    gaugeProvider: CLKGaugeProvider,
    bottomImageProvider: CLKFullColorImageProvider,
    centerTextProvider: CLKTextProvider
)
```

## Parameters 

`gaugeProvider`  

The gauge provider for the template.

`bottomImageProvider`  

The image provider for a small image at the bottom of the template. This template uses a full-color image.

`centerTextProvider`  

The text provider for the center text. The template supports multicolored text from this text provider.

