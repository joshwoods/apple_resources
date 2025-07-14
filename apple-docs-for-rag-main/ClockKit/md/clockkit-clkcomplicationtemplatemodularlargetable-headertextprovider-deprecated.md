

- ClockKit
- CLKComplicationTemplateModularLargeTable
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

var headerImageProvider: CLKImageProvider?

An optional image to display in the header.

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

var column2Alignment: CLKComplicationColumnAlignment

The alignment of the text in the second column.

Deprecated

