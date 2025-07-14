

- ClockKit
- CLKComplicationTemplateGraphicRectangularLargeImage
-  textProvider Deprecated

Instance Property

# textProvider

The header text to display in the complication.

watchOS 5.0–9.0Deprecated

``` source
@NSCopying
var textProvider: CLKTextProvider { get set }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

This property supports multicolor text.

In watchOS 5 and earlier, the system converts the text to uppercase before displaying it. In watchOS 6 and later, it displays the text using its original case.

## See Also

### Setting the Complication Data

var imageProvider: CLKFullColorImageProvider

The image to display.

Deprecated

