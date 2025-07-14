

- ClockKit
- CLKComplicationTemplateModularLargeStandardBody
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

The width of the header image determines how much space is available for displaying text. A tint color is applied to the header text to differentiate it from the body text rows. In multicolor environments, the text provider or template provide the tint color. In monochrome environments, the clock face provides the tint color.

## See Also

### Setting the Complication Data

var headerImageProvider: CLKImageProvider?

An optional image to display in the header.

Deprecated

var body1TextProvider: CLKTextProvider

The top line of body text.

Deprecated

var body2TextProvider: CLKTextProvider?

An optional second line of body text.

Deprecated

