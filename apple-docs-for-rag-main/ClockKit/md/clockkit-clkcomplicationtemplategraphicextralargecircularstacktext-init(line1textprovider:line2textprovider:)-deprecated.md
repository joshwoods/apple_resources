

- ClockKit
- CLKComplicationTemplateGraphicExtraLargeCircularStackText
-  init(line1TextProvider:line2TextProvider:) Deprecated

Initializer

# init(line1TextProvider:line2TextProvider:)

Creates a new template with two rows of text.

watchOS 7.0–9.0Deprecated

``` source
init(
    line1TextProvider: CLKTextProvider,
    line2TextProvider: CLKTextProvider
)
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Parameters 

`line1TextProvider`  

The text provider for the top row of text. The template supports multicolored text from this text provider.

`line2TextProvider`  

The text provider for the bottom row of text. The template supports multicolored text from this text provider.

