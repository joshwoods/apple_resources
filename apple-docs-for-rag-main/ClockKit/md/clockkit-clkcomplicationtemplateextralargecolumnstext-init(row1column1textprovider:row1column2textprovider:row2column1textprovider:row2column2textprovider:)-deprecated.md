

- ClockKit
- CLKComplicationTemplateExtraLargeColumnsText
-  init(row1Column1TextProvider:row1Column2TextProvider:row2Column1TextProvider:row2Column2TextProvider:) Deprecated

Initializer

# init(row1Column1TextProvider:row1Column2TextProvider:row2Column1TextProvider:row2Column2TextProvider:)

Creates a new template that has two columns of text.

watchOS 7.0–9.0Deprecated

``` source
init(
    row1Column1TextProvider: CLKTextProvider,
    row1Column2TextProvider: CLKTextProvider,
    row2Column1TextProvider: CLKTextProvider,
    row2Column2TextProvider: CLKTextProvider
)
```

## Parameters 

`row1Column1TextProvider`  

A text provider for the top row of the first column. For multicolor faces, like the Utility face, the system uses the text provider’s tint color for the text. For other faces, the system ignores the provided tint color, and uses a system color instead.

`row1Column2TextProvider`  

A text provider for the top row of the second column. For multicolor faces, like the Utility face, the system uses the text provider’s tint color for the text. For other faces, the system ignores the provided tint color, and uses a system color instead.

`row2Column1TextProvider`  

A text provider for the bottom row of the first column. For multicolor faces, like the Utility face, the system uses the text provider’s tint color for the text. For other faces, the system ignores the provided tint color, and uses a system color instead.

`row2Column2TextProvider`  

A text provider for the bottom row of the second column. For multicolor faces, like the Utility face, the system uses the text provider’s tint color for the text. For other faces, the system ignores the provided tint color, and uses a system color instead.

