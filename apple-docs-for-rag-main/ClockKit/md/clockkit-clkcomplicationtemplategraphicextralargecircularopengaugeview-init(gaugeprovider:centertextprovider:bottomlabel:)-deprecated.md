

- ClockKit
- CLKComplicationTemplateGraphicExtraLargeCircularOpenGaugeView
-  init(gaugeProvider:centerTextProvider:bottomLabel:) Deprecated

Initializer

# init(gaugeProvider:centerTextProvider:bottomLabel:)

Creates a new template that has an open circular gauge, a small amount of text in the center, and a small SwiftUI view at the bottom.

ClockKitSwiftUIwatchOS 7.0–9.0Deprecated

``` source
init(
    gaugeProvider: CLKGaugeProvider,
    centerTextProvider: CLKTextProvider,
    bottomLabel: Label
)
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Parameters 

`gaugeProvider`  

The gauge provider for the template.

`centerTextProvider`  

The text provider for the center text. The template supports multicolored text from this text provider.

`bottomLabel`  

The SwiftUI view displayed by the template.

