

- ClockKit
- CLKComplicationTemplateGraphicCircularStackImage
-  init(line1ImageProvider:line2TextProvider:) Deprecated

Initializer

# init(line1ImageProvider:line2TextProvider:)

Creates a template that has an image and a small amount of text.

watchOS 7.0–9.0Deprecated

``` source
init(
    line1ImageProvider: CLKFullColorImageProvider,
    line2TextProvider: CLKTextProvider
)
```

## Parameters 

`line1ImageProvider`  

A full-color image provider.

`line2TextProvider`  

The text provider for the text below the image. The template supports multicolored text from this text provider.

