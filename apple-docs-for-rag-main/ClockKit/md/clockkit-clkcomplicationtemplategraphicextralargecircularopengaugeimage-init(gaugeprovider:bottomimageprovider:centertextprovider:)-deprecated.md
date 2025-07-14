

- ClockKit
- CLKComplicationTemplateGraphicExtraLargeCircularOpenGaugeImage
-  init(gaugeProvider:bottomImageProvider:centerTextProvider:) Deprecated

Initializer

# init(gaugeProvider:bottomImageProvider:centerTextProvider:)

Creates a new template with an open circular gauge, an image at the bottom, and text in the center.

watchOS 7.0–9.0Deprecated

``` source
init(
    gaugeProvider: CLKGaugeProvider,
    bottomImageProvider: CLKFullColorImageProvider,
    centerTextProvider: CLKTextProvider
)
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Parameters 

`gaugeProvider`  

The gauge provider for the template.

`bottomImageProvider`  

The image provider for the image at the bottom of the template. This template uses a full-color image.

`centerTextProvider`  

The text provider for the center text. The template supports multicolored text from this text provider.

