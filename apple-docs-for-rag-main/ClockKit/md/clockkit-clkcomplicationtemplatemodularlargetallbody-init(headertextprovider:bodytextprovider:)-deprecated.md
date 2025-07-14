

- ClockKit
- CLKComplicationTemplateModularLargeTallBody
-  init(headerTextProvider:bodyTextProvider:) Deprecated

Initializer

# init(headerTextProvider:bodyTextProvider:)

Creates a template that has a header and a row of tall body text.

watchOS 7.0–9.0Deprecated

``` source
init(
    headerTextProvider: CLKTextProvider,
    bodyTextProvider: CLKTextProvider
)
```

## Parameters 

`headerTextProvider`  

The text provider for the header. For multicolor faces, like the Utility face, the system uses the text provider’s tint color for the text. For other faces, the system ignores the provided tint color, and uses a system color instead.

`bodyTextProvider`  

The text provider for the body. For multicolor faces, like the Utility face, the system uses the text provider’s tint color for the text. For other faces, the system ignores the provided tint color, and uses a system color instead.

