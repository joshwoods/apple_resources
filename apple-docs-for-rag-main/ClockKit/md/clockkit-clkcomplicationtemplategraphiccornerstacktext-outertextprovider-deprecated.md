

- ClockKit
- CLKComplicationTemplateGraphicCornerStackText
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

var innerTextProvider: CLKTextProvider

The inner text to display in the complication.

Deprecated

