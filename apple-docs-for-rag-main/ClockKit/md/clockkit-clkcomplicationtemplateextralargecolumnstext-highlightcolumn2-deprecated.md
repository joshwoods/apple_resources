

- ClockKit
- CLKComplicationTemplateExtraLargeColumnsText
-  highlightColumn2 Deprecated

Instance Property

# highlightColumn2

A Boolean value indicating which column should be drawn with a highlight.

watchOS 3.0–9.0Deprecated

``` source
var highlightColumn2: Bool { get set }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

When the value of this property is true, text in column two is rendered with a highlight. When the value is false, the text in column one is rendered with a highlight. The default value of this property is false.

## See Also

### Setting the Complication Data

var column2Alignment: CLKComplicationColumnAlignment

The alignment of the text in the second column.

Deprecated

var row1Column1TextProvider: CLKTextProvider

The text to display in the first column of the first row.

Deprecated

var row1Column2TextProvider: CLKTextProvider

The text to display in the second column of the first row.

Deprecated

var row2Column1TextProvider: CLKTextProvider

The text to display in the first column of the second row.

Deprecated

var row2Column2TextProvider: CLKTextProvider

The text to display in the second column of the second row.

Deprecated

