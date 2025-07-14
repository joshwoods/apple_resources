

- ClockKit
- CLKComplicationTemplateGraphicCornerGaugeText
-  outerTextProvider Deprecated

Instance Property

# outerTextProvider

The outer text to display in the complication.

watchOS 5.0–9.0Deprecated

``` source
@NSCopying
var outerTextProvider: CLKTextProvider { get set }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

The complication ignores the text provider’s tint color. It always displays the outer text as white.

## See Also

### Setting the Complication Data

var gaugeProvider: CLKGaugeProvider

The gauge to display in the complication.

Deprecated

var leadingTextProvider: CLKTextProvider?

The text to display on the leading edge of the gague.

Deprecated

var trailingTextProvider: CLKTextProvider?

The text to display on the trailing edge of the gauge.

Deprecated

