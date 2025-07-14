

- ClockKit
- CLKComplicationTemplateModularLargeTable
-  init(headerImageProvider:headerTextProvider:row1Column1TextProvider:row1Column2TextProvider:row2Column1TextProvider:row2Column2TextProvider:) Deprecated

Initializer

# init(headerImageProvider:headerTextProvider:row1Column1TextProvider:row1Column2TextProvider:row2Column1TextProvider:row2Column2TextProvider:)

Creates a template that has a header row with an image and text, and two columns of text.

watchOS 7.0–9.0Deprecated

``` source
init(
    headerImageProvider: CLKImageProvider?,
    headerTextProvider: CLKTextProvider,
    row1Column1TextProvider: CLKTextProvider,
    row1Column2TextProvider: CLKTextProvider,
    row2Column1TextProvider: CLKTextProvider,
    row2Column2TextProvider: CLKTextProvider
)
```

## Parameters 

`headerImageProvider`  

The image provider for the header image. The system renders the image as a tinted template image, a bitmap image where only the opacity of the image matters. For more information, see Providing images for different appearances.

`headerTextProvider`  

The text provider for the header text. For multicolor faces, like the Utility face, the system uses the text provider’s tint color for the text. For other faces, the system ignores the provided tint color, and uses a system color instead.

`row1Column1TextProvider`  

The text provider for the first row of the first column. For multicolor faces, like the Utility face, the system uses the text provider’s tint color for the text. For other faces, the system ignores the provided tint color, and uses a system color instead.

`row1Column2TextProvider`  

The text provider for the first row of the second column. For multicolor faces, like the Utility face, the system uses the text provider’s tint color for the text. For other faces, the system ignores the provided tint color, and uses a system color instead.

`row2Column1TextProvider`  

The text provider for the second row of the first column. For multicolor faces, like the Utility face, the system uses the text provider’s tint color for the text. For other faces, the system ignores the provided tint color, and uses a system color instead.

`row2Column2TextProvider`  

The text provider for the second row of the second column. For multicolor faces, like the Utility face, the system uses the text provider’s tint color for the text. For other faces, the system ignores the provided tint color, and uses a system color instead.

## See Also

### Creating the Template

init(headerTextProvider: CLKTextProvider, row1Column1TextProvider: CLKTextProvider, row1Column2TextProvider: CLKTextProvider, row2Column1TextProvider: CLKTextProvider, row2Column2TextProvider: CLKTextProvider)

Creates a template that has a header and two columns of text.

Deprecated

