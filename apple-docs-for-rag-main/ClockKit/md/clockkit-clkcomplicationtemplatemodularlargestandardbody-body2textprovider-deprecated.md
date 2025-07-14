

- ClockKit
- CLKComplicationTemplateModularLargeStandardBody
-  body2TextProvider Deprecated

Instance Property

# body2TextProvider

An optional second line of body text.

watchOS 2.0–9.0Deprecated

``` source
@NSCopying
var body2TextProvider: CLKTextProvider? { get set }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

If you don’t specify a value for this property, the text in the body1TextProvider property wraps and is displayed on the second line.

## See Also

### Setting the Complication Data

var headerImageProvider: CLKImageProvider?

An optional image to display in the header.

Deprecated

var headerTextProvider: CLKTextProvider

The text to display in the header line.

Deprecated

var body1TextProvider: CLKTextProvider

The top line of body text.

Deprecated

