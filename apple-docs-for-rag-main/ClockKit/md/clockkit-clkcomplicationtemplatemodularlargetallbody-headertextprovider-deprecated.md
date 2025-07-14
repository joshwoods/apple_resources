

- ClockKit
- CLKComplicationTemplateModularLargeTallBody
-  headerTextProvider Deprecated

Instance Property

# headerTextProvider

The text to display in the header line.

watchOS 2.0–9.0Deprecated

``` source
@NSCopying
var headerTextProvider: CLKTextProvider { get set }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

A tint color is applied to the header text to differentiate it from the other rows. In multicolor environments, the text provider or template provide the tint color. In monochrome environments, the clock face provides the tint color.

## See Also

### Setting the Complication Data

var bodyTextProvider: CLKTextProvider

The text to display in the body line.

Deprecated

