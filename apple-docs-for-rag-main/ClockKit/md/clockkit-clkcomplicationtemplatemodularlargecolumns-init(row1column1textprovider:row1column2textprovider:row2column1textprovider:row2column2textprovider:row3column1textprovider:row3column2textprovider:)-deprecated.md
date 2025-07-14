

- ClockKit
- CLKComplicationTemplateModularLargeColumns
-  init(row1Column1TextProvider:row1Column2TextProvider:row2Column1TextProvider:row2Column2TextProvider:row3Column1TextProvider:row3Column2TextProvider:) Deprecated

Initializer

# init(row1Column1TextProvider:row1Column2TextProvider:row2Column1TextProvider:row2Column2TextProvider:row3Column1TextProvider:row3Column2TextProvider:)

Creates a template that has two columns of text.

watchOS 7.0–9.0Deprecated

``` source
init(
    row1Column1TextProvider: CLKTextProvider,
    row1Column2TextProvider: CLKTextProvider,
    row2Column1TextProvider: CLKTextProvider,
    row2Column2TextProvider: CLKTextProvider,
    row3Column1TextProvider: CLKTextProvider,
    row3Column2TextProvider: CLKTextProvider
)
```

## Parameters 

`row1Column1TextProvider`  

The text provider for the first row in the first column. For multicolor faces, like the Utility face, the system uses the text provider’s tint color for the text. For other faces, the system ignores the provided tint color, and uses a system color instead.

`row1Column2TextProvider`  

The text provider for the first row in the second column. For multicolor faces, like the Utility face, the system uses the text provider’s tint color for the text. For other faces, the system ignores the provided tint color, and uses a system color instead.

`row2Column1TextProvider`  

The text provider for the second row in the first column. For multicolor faces, like the Utility face, the system uses the text provider’s tint color for the text. For other faces, the system ignores the provided tint color, and uses a system color instead.

`row2Column2TextProvider`  

The text provider for the second row in the second column. For multicolor faces, like the Utility face, the system uses the text provider’s tint color for the text. For other faces, the system ignores the provided tint color, and uses a system color instead.

`row3Column1TextProvider`  

The text provider for the third row in the first column. For multicolor faces, like the Utility face, the system uses the text provider’s tint color for the text. For other faces, the system ignores the provided tint color, and uses a system color instead.

`row3Column2TextProvider`  

The text provider for the third row in the second column. For multicolor faces, like the Utility face, the system uses the text provider’s tint color for the text. For other faces, the system ignores the provided tint color, and uses a system color instead.

## See Also

### Creating the Template

init(row1ImageProvider: CLKImageProvider?, row1Column1TextProvider: CLKTextProvider, row1Column2TextProvider: CLKTextProvider, row2ImageProvider: CLKImageProvider?, row2Column1TextProvider: CLKTextProvider, row2Column2TextProvider: CLKTextProvider, row3ImageProvider: CLKImageProvider?, row3Column1TextProvider: CLKTextProvider, row3Column2TextProvider: CLKTextProvider)

Creates a template that has a column of images and two columns of text.

Deprecated

