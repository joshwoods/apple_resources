

- ClockKit
- CLKComplicationTemplateGraphicRectangularStandardBody
-  init(headerTextProvider:body1TextProvider:body2TextProvider:) Deprecated

Initializer

# init(headerTextProvider:body1TextProvider:body2TextProvider:)

Creates a new template that has a row of header text and two rows of body text.

watchOS 7.0–9.0Deprecated

``` source
init(
    headerTextProvider: CLKTextProvider,
    body1TextProvider: CLKTextProvider,
    body2TextProvider: CLKTextProvider?
)
```

## Parameters 

`headerTextProvider`  

The text provider for the header text. The template supports multicolored text from this text provider.

`body1TextProvider`  

The text provider for the first row of body text. The template supports multicolored text from this text provider.

`body2TextProvider`  

The text provider for the second row of body text. The template supports multicolored text from this text provider.

## See Also

### Creating the Template

init(headerTextProvider: CLKTextProvider, body1TextProvider: CLKTextProvider)

Creates a new template that has a row of header text and a row of body text.

Deprecated

init(headerImageProvider: CLKFullColorImageProvider?, headerTextProvider: CLKTextProvider, body1TextProvider: CLKTextProvider)

Creates a new template that has a header row with an image and text, and a row of body text.

Deprecated

init(headerImageProvider: CLKFullColorImageProvider?, headerTextProvider: CLKTextProvider, body1TextProvider: CLKTextProvider, body2TextProvider: CLKTextProvider?)

Creates a new template that has a header row with an image and text, and two rows of body text.

Deprecated

