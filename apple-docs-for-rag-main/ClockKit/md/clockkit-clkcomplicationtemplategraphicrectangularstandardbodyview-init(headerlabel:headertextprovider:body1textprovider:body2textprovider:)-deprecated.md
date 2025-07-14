

- ClockKit
- CLKComplicationTemplateGraphicRectangularStandardBodyView
-  init(headerLabel:headerTextProvider:body1TextProvider:body2TextProvider:) Deprecated

Initializer

# init(headerLabel:headerTextProvider:body1TextProvider:body2TextProvider:)

Creates a new template that has a header row with a SwiftUI view and text, and two rows of body text.

ClockKitSwiftUIwatchOS 7.0–9.0Deprecated

``` source
init(
    headerLabel: Label,
    headerTextProvider: CLKTextProvider,
    body1TextProvider: CLKTextProvider,
    body2TextProvider: CLKTextProvider? = nil
)
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Parameters 

`headerLabel`  

The SwiftUI view displayed by the template.

`headerTextProvider`  

The text provider for the header text. The template supports multicolored text from this text provider.

`body1TextProvider`  

The text provider for the first row of body text. The template supports multicolored text from this text provider.

`body2TextProvider`  

The text provider for the second row of body text. The template supports multicolored text from this text provider.

