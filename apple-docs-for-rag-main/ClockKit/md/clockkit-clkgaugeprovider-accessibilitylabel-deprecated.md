

- ClockKit
- CLKGaugeProvider
-  accessibilityLabel Deprecated

Instance Property

# accessibilityLabel

A localized string that describes the gague.

watchOS 5.0–9.0Deprecated

``` source
var accessibilityLabel: String? { get set }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

Set this property to provide a succinct description for the gauge. VoiceOver reads this property when describing the gauge. By default, this property is `nil`.

