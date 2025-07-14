

- ClockKit
- CLKComplicationTemplateModularLargeStandardBody
-  body1TextProvider Deprecated

Instance Property

# body1TextProvider

The top line of body text.

watchOS 2.0–9.0Deprecated

``` source
@NSCopying
var body1TextProvider: CLKTextProvider { get set }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

If you don’t specify a value for the body2TextProvider property, the text in this property wraps to the second line.

## See Also

### Setting the Complication Data

var headerImageProvider: CLKImageProvider?

An optional image to display in the header.

Deprecated

var headerTextProvider: CLKTextProvider

The text to display in the header line.

Deprecated

var body2TextProvider: CLKTextProvider?

An optional second line of body text.

Deprecated

