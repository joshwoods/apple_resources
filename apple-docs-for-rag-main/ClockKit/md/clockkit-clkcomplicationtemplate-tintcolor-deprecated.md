

- ClockKit
- CLKComplicationTemplate
-  tintColor Deprecated

Instance Property

# tintColor

The tint color to apply to elements of the template.

watchOS 2.0–9.0Deprecated

``` source
@NSCopying
var tintColor: UIColor? { get set }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

The color in this property is the default color applied to images and highlighted text in the template. This color is applied only on clock faces that support multiple colors and only when the text or image provider doesn’t provide a custom color. If the value in this property is `nil`, ClockKit uses white for the default color.

