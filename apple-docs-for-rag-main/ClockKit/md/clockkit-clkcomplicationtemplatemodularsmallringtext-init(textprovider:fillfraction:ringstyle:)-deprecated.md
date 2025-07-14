

- ClockKit
- CLKComplicationTemplateModularSmallRingText
-  init(textProvider:fillFraction:ringStyle:) Deprecated

Initializer

# init(textProvider:fillFraction:ringStyle:)

Creates a new template from the provided text, fill fraction, and ring style.

watchOS 7.0–9.0Deprecated

``` source
init(
    textProvider: CLKTextProvider,
    fillFraction: Float,
    ringStyle: CLKComplicationRingStyle
)
```

## Parameters 

`textProvider`  

A text provider for the text in the center of the template. For multicolor faces, like the Utility face, the system uses the text provider’s tint color for the text. For other faces, the system ignores the provided tint color, and uses a system color instead.

`fillFraction`  

A value between `0.0` and `1.0` that indicates how much of the ring fills.

`ringStyle`  

The ring’s style. For a complete list of styles, see CLKComplicationRingStyle.

