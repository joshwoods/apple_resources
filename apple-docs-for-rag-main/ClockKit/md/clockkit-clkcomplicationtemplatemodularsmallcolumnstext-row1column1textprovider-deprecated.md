

- ClockKit
- CLKComplicationTemplateModularSmallColumnsText
-  row1Column1TextProvider Deprecated

Instance Property

# row1Column1TextProvider

The text to display in the first column of the first row.

watchOS 2.0–9.0Deprecated

``` source
@NSCopying
var row1Column1TextProvider: CLKTextProvider { get set }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

When the highlightColumn2 property is false, a tint color is applied to this text. In multicolor environments, the text provider or template provide the tint color. In monochrome environments, the clock face provides the tint color.

## See Also

### Setting the Complication Data

var row1Column2TextProvider: CLKTextProvider

The text to display in the second column of the first row.

Deprecated

var row2Column1TextProvider: CLKTextProvider

The text to display in the first column of the second row.

Deprecated

var row2Column2TextProvider: CLKTextProvider

The text to display in the second column of the second row.

Deprecated

var column2Alignment: CLKComplicationColumnAlignment

The alignment of the text in the second column.

Deprecated

var highlightColumn2: Bool

A Boolean value indicating which column should be drawn with a highlight.

Deprecated

