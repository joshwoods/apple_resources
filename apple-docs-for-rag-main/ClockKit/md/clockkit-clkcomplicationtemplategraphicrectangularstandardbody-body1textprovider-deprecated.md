

- ClockKit
- CLKComplicationTemplateGraphicRectangularStandardBody
-  body1TextProvider Deprecated

Instance Property

# body1TextProvider

The main body text to display in the complication.

watchOS 5.0–9.0Deprecated

``` source
@NSCopying
var body1TextProvider: CLKTextProvider { get set }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

In watchOS 5 and earlier, the system always displays the text as white. In watchOS 6 and later, it can display multicolor text.

## See Also

### Setting the Complication Data

var headerTextProvider: CLKTextProvider

The header text to display in the complication.

Deprecated

var headerImageProvider: CLKFullColorImageProvider?

The header image to display.

Deprecated

var body2TextProvider: CLKTextProvider?

The secondary body text to display in the complication.

Deprecated

