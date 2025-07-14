

- ClockKit
- CLKComplicationTemplateCircularSmallStackImage
-  init(line1ImageProvider:line2TextProvider:) Deprecated

Initializer

# init(line1ImageProvider:line2TextProvider:)

Creates a new template from the provided image and text.

watchOS 7.0–9.0Deprecated

``` source
init(
    line1ImageProvider: CLKImageProvider,
    line2TextProvider: CLKTextProvider
)
```

## Parameters 

`line1ImageProvider`  

The image provider for the main image. The system renders the image as a tinted template image a bitmap image where only the opacity of the image matters. For more information, see Providing images for different appearances.

`line2TextProvider`  

The text provider for the text below the image. For multicolor faces, like the Utility face, the system uses the text provider’s tint color for the text. For other faces, the system ignores the provided tint color, and uses a system color instead.

