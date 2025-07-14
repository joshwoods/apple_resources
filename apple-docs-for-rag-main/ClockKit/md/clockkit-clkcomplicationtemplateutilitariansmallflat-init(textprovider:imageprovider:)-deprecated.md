

- ClockKit
- CLKComplicationTemplateUtilitarianSmallFlat
-  init(textProvider:imageProvider:) Deprecated

Initializer

# init(textProvider:imageProvider:)

Creates a new template that has a single row with an image and a line of text.

watchOS 7.0–9.0Deprecated

``` source
init(
    textProvider: CLKTextProvider,
    imageProvider: CLKImageProvider?
)
```

## Parameters 

`textProvider`  

The text provider for the line of text. For multicolor faces, like the Utility face, the system uses the text provider’s tint color for the text. For other faces, the system ignores the provided tint color, and uses a system color instead.

`imageProvider`  

The image provider for the leading image. The system renders the image as a tinted template image, a bitmap image where only the opacity of the image matters. For more information, see Providing images for different appearances.

## See Also

### Creating the Template

init(textProvider: CLKTextProvider)

Creates a new template that has a single line of text.

Deprecated

