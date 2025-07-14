

- ClockKit
- CLKComplicationTemplateCircularSmallStackText
-  init(line1TextProvider:line2TextProvider:) Deprecated

Initializer

# init(line1TextProvider:line2TextProvider:)

Creates a new template that has two lines of text.

watchOS 7.0–9.0Deprecated

``` source
init(
    line1TextProvider: CLKTextProvider,
    line2TextProvider: CLKTextProvider
)
```

## Parameters 

`line1TextProvider`  

A text provider for the top line of text. For multicolor faces, like the Utility face, the system uses the text provider’s tint color for the text. For other faces, the system ignores the provided tint color, and uses a system color instead.

`line2TextProvider`  

A text provider for the bottom line of text. For multicolor faces, like the Utility face, the system uses the text provider’s tint color for the text. For other faces, the system ignores the provided tint color, and uses a system color instead.

