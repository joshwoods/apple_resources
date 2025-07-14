

- ClockKit
- CLKComplicationTemplateCircularSmallSimpleText
-  init(textProvider:) Deprecated

Initializer

# init(textProvider:)

Creates a new template from the provided text.

watchOS 7.0–9.0Deprecated

``` source
init(textProvider: CLKTextProvider)
```

## Parameters 

`textProvider`  

A text provider for the text in the center of the template. For multicolor faces, like the Utility face, the system uses the text provider’s tint color for the text. For other faces, the system ignores the provided tint color, and uses a system color instead.

