

- ClockKit
- CLKComplicationTemplateModularLargeStandardBody
-  headerImageProvider Deprecated

Instance Property

# headerImageProvider

An optional image to display in the header.

watchOS 2.0–9.0Deprecated

``` source
@NSCopying
var headerImageProvider: CLKImageProvider? { get set }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

A tint color is applied to the header image to differentiate it from the other rows. In multicolor environments, the image provider or template provide the tint color. In monochrome environments, the clock face provides the tint color.

## See Also

### Setting the Complication Data

var headerTextProvider: CLKTextProvider

The text to display in the header line.

Deprecated

var body1TextProvider: CLKTextProvider

The top line of body text.

Deprecated

var body2TextProvider: CLKTextProvider?

An optional second line of body text.

Deprecated

