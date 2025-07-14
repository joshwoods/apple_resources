

- ClockKit
- CLKComplicationTemplateGraphicCornerGaugeView
-  init(gaugeProvider:leadingTextProvider:trailingTextProvider:label:) Deprecated

Initializer

# init(gaugeProvider:leadingTextProvider:trailingTextProvider:label:)

Creates a new template with the provided gauge and view.

ClockKitSwiftUIwatchOS 7.0–9.0Deprecated

``` source
init(
    gaugeProvider: CLKGaugeProvider,
    leadingTextProvider: CLKTextProvider? = nil,
    trailingTextProvider: CLKTextProvider? = nil,
    label: Label
)
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Parameters 

`gaugeProvider`  

The gauge provider for the template.

`leadingTextProvider`  

The text provider for the gauge’s leading text. The template supports multicolored text from this text provider.

`trailingTextProvider`  

The text provider for the gauge’s trailing text. The template supports multicolored text from this text provider.

`label`  

The SwiftUI view displayed by the template.

