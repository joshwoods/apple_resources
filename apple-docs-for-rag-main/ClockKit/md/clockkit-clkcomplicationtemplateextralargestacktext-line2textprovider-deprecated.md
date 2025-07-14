

- ClockKit
- CLKComplicationTemplateExtraLargeStackText
-  line2TextProvider Deprecated

Instance Property

# line2TextProvider

The text to display on the bottom line of the complication.

watchOS 3.0–9.0Deprecated

``` source
@NSCopying
var line2TextProvider: CLKTextProvider { get set }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

Space for text is limited in this particular template so keep strings as short as possible.

When the highlightLine2 property is true, a tint color is applied to this text. In multicolor environments, the text provider or template provides the tint color. In monochrome environments, the clock face provides the tint color.

## See Also

### Setting the Complication Data

var highlightLine2: Bool

A Boolean value indicating which line should be drawn with a highlight.

Deprecated

var line1TextProvider: CLKTextProvider

The text to display on the top line of the complication.

Deprecated

