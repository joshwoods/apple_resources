

- ClockKit
- CLKComplicationTemplateGraphicCornerGaugeImage
-  init(gaugeProvider:leadingTextProvider:trailingTextProvider:imageProvider:) Deprecated

Initializer

# init(gaugeProvider:leadingTextProvider:trailingTextProvider:imageProvider:)

Creates a new template that has a gauge with leading and trailing text and an image.

watchOS 7.0–9.0Deprecated

``` source
init(
    gaugeProvider: CLKGaugeProvider,
    leadingTextProvider: CLKTextProvider?,
    trailingTextProvider: CLKTextProvider?,
    imageProvider: CLKFullColorImageProvider
)
```

## Parameters 

`gaugeProvider`  

The gauge provider for the template.

`leadingTextProvider`  

The text provider for the gauge’s leading text. The template supports multicolored text from this text provider.

`trailingTextProvider`  

The text provider for the gauge’s trailing text. The template supports multicolored text from this text provider.

`imageProvider`  

A full-color image provider.

## See Also

### Creating the Template

init(gaugeProvider: CLKGaugeProvider, imageProvider: CLKFullColorImageProvider)

Creates a new template that has a gauge and an image.

Deprecated

