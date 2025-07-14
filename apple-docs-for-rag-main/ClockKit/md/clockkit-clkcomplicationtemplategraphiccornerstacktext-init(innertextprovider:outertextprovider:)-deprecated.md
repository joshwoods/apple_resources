

- ClockKit
- CLKComplicationTemplateGraphicCornerStackText
-  init(innerTextProvider:outerTextProvider:) Deprecated

Initializer

# init(innerTextProvider:outerTextProvider:)

Creates a template that has an inner line of text and an outer text element.

watchOS 7.0–9.0Deprecated

``` source
init(
    innerTextProvider: CLKTextProvider,
    outerTextProvider: CLKTextProvider
)
```

## Parameters 

`innerTextProvider`  

The text provider for the inner line of text. The template supports multicolored text from this text provider.

`outerTextProvider`  

The text provider for the outer line of text. The template ignores this text provider’s tint color, and always displays the text with a system color.

