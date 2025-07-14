

- ClockKit
-  CLKComplicationTemplateModularLargeTable Deprecated

Class

# CLKComplicationTemplateModularLargeTable

A template for displaying a header row and columns.

watchOS 2.0–9.0Deprecated

``` source
class CLKComplicationTemplateModularLargeTable
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.modularLarge family.

The following table lists the dimensions of the image you use in this template. All dimensions are in pixels. All images must be specified as `@2x` images for display on Apple Watch, so the point-based dimensions are half the listed size. The width of the image must be between the specified minimum and maximum (inclusive).

| Apple Watch Size | Width | Height |
|----|----|----|
| 38 mm | 22 pixels minimum  64 pixels maximum | 22 pixels |
| 40 mm | 24 pixels minimum  74 pixels maximum | 24 pixels |
| 41 mm | 25 pixels minimum  78 pixels maximum | 25 pixels |
| 42 mm | 24 pixels minimum  74 pixels maximum | 24 pixels |
| 44 mm | 28 pixels minimum  84 pixels maximum | 28 pixels |
| 45 mm | 29 pixels minimum  88 pixels maximum | 29 pixels |

Instead of providing multiple images with different resolutions, you can provide a single, scaleable PDF asset. For more information, see `Manage Assets`.

## Topics

### Creating the Template

init(headerTextProvider: CLKTextProvider, row1Column1TextProvider: CLKTextProvider, row1Column2TextProvider: CLKTextProvider, row2Column1TextProvider: CLKTextProvider, row2Column2TextProvider: CLKTextProvider)

Creates a template that has a header and two columns of text.

init(headerImageProvider: CLKImageProvider?, headerTextProvider: CLKTextProvider, row1Column1TextProvider: CLKTextProvider, row1Column2TextProvider: CLKTextProvider, row2Column1TextProvider: CLKTextProvider, row2Column2TextProvider: CLKTextProvider)

Creates a template that has a header row with an image and text, and two columns of text.

### Setting the Complication Data

var headerImageProvider: CLKImageProvider?

An optional image to display in the header.

var headerTextProvider: CLKTextProvider

The text to display in the header line.

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

### Table templates

class CLKComplicationTemplateModularLargeColumns

A template for displaying multiple columns of data.

Deprecated

