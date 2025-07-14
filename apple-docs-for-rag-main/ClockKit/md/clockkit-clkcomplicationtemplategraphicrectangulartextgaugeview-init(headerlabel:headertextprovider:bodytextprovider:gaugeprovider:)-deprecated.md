

- ClockKit
- CLKComplicationTemplateGraphicRectangularTextGaugeView
-  init(headerLabel:headerTextProvider:bodyTextProvider:gaugeProvider:) Deprecated

Initializer

# init(headerLabel:headerTextProvider:bodyTextProvider:gaugeProvider:)

Creates a new template that has a header row with a SwiftUI view and text, body text, and a gauge.

ClockKitSwiftUIwatchOS 7.0–9.0Deprecated

``` source
init(
    headerLabel: Label,
    headerTextProvider: CLKTextProvider,
    bodyTextProvider: CLKTextProvider,
    gaugeProvider: CLKGaugeProvider
)
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Parameters 

`headerLabel`  

The SwiftUI view displayed by the template.

`headerTextProvider`  

The text provider for the header text. The template supports multicolored text from this text provider.

`bodyTextProvider`  

The text provider for the body text. The template supports multicolored text from this text provider.

`gaugeProvider`  

The gauge provider for the template.

