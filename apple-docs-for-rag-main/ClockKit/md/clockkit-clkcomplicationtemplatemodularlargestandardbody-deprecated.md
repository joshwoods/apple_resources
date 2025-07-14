

- ClockKit
-  CLKComplicationTemplateModularLargeStandardBody Deprecated

Class

# CLKComplicationTemplateModularLargeStandardBody

A template for displaying a header row and two lines of text.

watchOS 2.0–9.0Deprecated

``` source
class CLKComplicationTemplateModularLargeStandardBody
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

init(headerTextProvider: CLKTextProvider, body1TextProvider: CLKTextProvider)

Creates a new template that has a row of header text and a row of body text.

init(headerTextProvider: CLKTextProvider, body1TextProvider: CLKTextProvider, body2TextProvider: CLKTextProvider?)

Creates a new template that has a row of header text and two rows of body text.

init(headerImageProvider: CLKImageProvider?, headerTextProvider: CLKTextProvider, body1TextProvider: CLKTextProvider)

Creates a new template that has a header row with an image and text, and a row of body text.

init(headerImageProvider: CLKImageProvider?, headerTextProvider: CLKTextProvider, body1TextProvider: CLKTextProvider, body2TextProvider: CLKTextProvider?)

Creates a new template that has a header row with an image and text, and two rows of body text.

### Setting the Complication Data

var headerImageProvider: CLKImageProvider?

An optional image to display in the header.

var headerTextProvider: CLKTextProvider

The text to display in the header line.

var body1TextProvider: CLKTextProvider

The top line of body text.

var body2TextProvider: CLKTextProvider?

An optional second line of body text.

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

### Body templates

class CLKComplicationTemplateModularLargeTallBody

A template for displaying a header row and row of tall body text.

Deprecated

