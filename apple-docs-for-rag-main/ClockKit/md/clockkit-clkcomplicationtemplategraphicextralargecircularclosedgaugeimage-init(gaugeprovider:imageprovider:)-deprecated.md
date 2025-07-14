

- ClockKit
- CLKComplicationTemplateGraphicExtraLargeCircularClosedGaugeImage
-  init(gaugeProvider:imageProvider:) Deprecated

Initializer

# init(gaugeProvider:imageProvider:)

Creates a new template with a closed circular gauge and an image in the center.

watchOS 7.0–9.0Deprecated

``` source
init(
    gaugeProvider: CLKGaugeProvider,
    imageProvider: CLKFullColorImageProvider
)
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Parameters 

`gaugeProvider`  

The gauge provider for the template.

`imageProvider`  

The image provider for the image at the center of the template. This template uses a full-color image.

