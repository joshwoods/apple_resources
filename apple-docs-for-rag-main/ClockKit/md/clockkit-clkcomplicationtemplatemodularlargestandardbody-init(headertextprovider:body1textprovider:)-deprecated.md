

- ClockKit
- CLKComplicationTemplateModularLargeStandardBody
-  init(headerTextProvider:body1TextProvider:) Deprecated

Initializer

# init(headerTextProvider:body1TextProvider:)

Creates a new template that has a row of header text and a row of body text.

watchOS 7.0–9.0Deprecated

``` source
init(
    headerTextProvider: CLKTextProvider,
    body1TextProvider: CLKTextProvider
)
```

## Parameters 

`headerTextProvider`  

The text provider for the header. For multicolor faces, like the Utility face, the system uses the text provider’s tint color for the text. For other faces, the system ignores the provided tint color, and uses a system color instead.

`body1TextProvider`  

The text provider for the row of body text. For multicolor faces, like the Utility face, the system uses the text provider’s tint color for the text. For other faces, the system ignores the provided tint color, and uses a system color instead.

## See Also

### Creating the Template

init(headerTextProvider: CLKTextProvider, body1TextProvider: CLKTextProvider, body2TextProvider: CLKTextProvider?)

Creates a new template that has a row of header text and two rows of body text.

Deprecated

init(headerImageProvider: CLKImageProvider?, headerTextProvider: CLKTextProvider, body1TextProvider: CLKTextProvider)

Creates a new template that has a header row with an image and text, and a row of body text.

Deprecated

init(headerImageProvider: CLKImageProvider?, headerTextProvider: CLKTextProvider, body1TextProvider: CLKTextProvider, body2TextProvider: CLKTextProvider?)

Creates a new template that has a header row with an image and text, and two rows of body text.

Deprecated

