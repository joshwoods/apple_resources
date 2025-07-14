

- ClockKit
-  CLKComplicationTemplateModularSmallColumnsText Deprecated

Class

# CLKComplicationTemplateModularSmallColumnsText

A template for displaying two rows and two columns of text.

watchOS 2.0–9.0Deprecated

``` source
class CLKComplicationTemplateModularSmallColumnsText
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.modularSmall family.

## Topics

### Creating the Template

init(row1Column1TextProvider: CLKTextProvider, row1Column2TextProvider: CLKTextProvider, row2Column1TextProvider: CLKTextProvider, row2Column2TextProvider: CLKTextProvider)

Creates a new template that has two columns of text.

### Setting the Complication Data

var row1Column1TextProvider: CLKTextProvider

The text to display in the first column of the first row.

var row1Column2TextProvider: CLKTextProvider

The text to display in the second column of the first row.

var row2Column1TextProvider: CLKTextProvider

The text to display in the first column of the second row.

var row2Column2TextProvider: CLKTextProvider

The text to display in the second column of the second row.

var column2Alignment: CLKComplicationColumnAlignment

The alignment of the text in the second column.

var highlightColumn2: Bool

A Boolean value indicating which column should be drawn with a highlight.

## Relationships

### Inherits From

- CLKComplicationTemplate

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Text templates

class CLKComplicationTemplateModularSmallRingText

A template for displaying text encircled by a configurable progress ring.

Deprecated

class CLKComplicationTemplateModularSmallSimpleText

A template for displaying a small amount of text.

Deprecated

class CLKComplicationTemplateModularSmallStackText

A template for displaying two strings stacked one on top of the other.

Deprecated

