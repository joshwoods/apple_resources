

- ClockKit
- CLKComplicationTemplateGraphicRectangularStandardBody
-  init(headerImageProvider:headerTextProvider:body1TextProvider:) Deprecated

Initializer

# init(headerImageProvider:headerTextProvider:body1TextProvider:)

Creates a new template that has a header row with an image and text, and a row of body text.

watchOS 7.0–9.0Deprecated

``` source
init(
    headerImageProvider: CLKFullColorImageProvider?,
    headerTextProvider: CLKTextProvider,
    body1TextProvider: CLKTextProvider
)
```

## Parameters 

`headerImageProvider`  

A full-color image provider.

`headerTextProvider`  

The text provider for the header text. The template supports multicolored text from this text provider.

`body1TextProvider`  

The text provider for the first row of body text. The template supports multicolored text from this text provider.

## See Also

### Creating the Template

init(headerTextProvider: CLKTextProvider, body1TextProvider: CLKTextProvider)

Creates a new template that has a row of header text and a row of body text.

Deprecated

init(headerTextProvider: CLKTextProvider, body1TextProvider: CLKTextProvider, body2TextProvider: CLKTextProvider?)

Creates a new template that has a row of header text and two rows of body text.

Deprecated

init(headerImageProvider: CLKFullColorImageProvider?, headerTextProvider: CLKTextProvider, body1TextProvider: CLKTextProvider, body2TextProvider: CLKTextProvider?)

Creates a new template that has a header row with an image and text, and two rows of body text.

Deprecated

