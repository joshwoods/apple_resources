

- ClockKit
- CLKComplicationTemplateExtraLargeStackImage
-  highlightLine2 Deprecated

Instance Property

# highlightLine2

A Boolean value indicating which line should be drawn with a highlight.

watchOS 3.0–9.0Deprecated

``` source
var highlightLine2: Bool { get set }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

When the value of this property is true, the text in row two is rendered with a highlight. When the value is false, the image on line one is rendered with a highlight. The default value of this property is false.

## See Also

### Setting the Complication Data

var line1ImageProvider: CLKImageProvider

The image to display on the top line of the complication.

Deprecated

var line2TextProvider: CLKTextProvider

The text to display on the bottom line of the complication.

Deprecated

