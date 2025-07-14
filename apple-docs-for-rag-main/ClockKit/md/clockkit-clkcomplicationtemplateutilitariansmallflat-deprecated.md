

- ClockKit
-  CLKComplicationTemplateUtilitarianSmallFlat Deprecated

Class

# CLKComplicationTemplateUtilitarianSmallFlat

A template for displaying an image and text in a single line.

watchOS 2.0–9.0Deprecated

``` source
class CLKComplicationTemplateUtilitarianSmallFlat
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.utilitarianSmall family.

The following table lists the dimensions of the image you use in this template. All dimensions are in pixels. All images must be specified as `@2x` images for display on Apple Watch, so the point-based dimensions are half the listed size. The width of the image must be between the specified minimum and maximum (inclusive).

| Apple Watch Size | Width | Height |
|----|----|----|
| 38 mm | 18 pixels minimum  42 pixels maximum | 18 pixels |
| 40 mm | 20 pixels minimum  44 pixels maximum | 20 pixels |
| 41 mm | 21 pixels minimum  47 pixels maximum | 21 pixels |
| 42 mm | 20 pixels minimum  44 pixels maximum | 20 pixels |
| 44 mm | 22 pixels minimum  49 pixels maximum | 22 pixels |
| 45 mm | 24 pixels minimum  52 pixels maximum | 24 pixels |

Instead of providing multiple images with different resolutions, you can provide a single, scaleable PDF asset. For more information, see `Manage Assets`.

## Topics

### Creating the Template

init(textProvider: CLKTextProvider)

Creates a new template that has a single line of text.

init(textProvider: CLKTextProvider, imageProvider: CLKImageProvider?)

Creates a new template that has a single row with an image and a line of text.

### Setting the Complication Data

var imageProvider: CLKImageProvider?

The image to display.

var textProvider: CLKTextProvider

The text to display.

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

### Utilitarian small

class CLKComplicationTemplateUtilitarianSmallRingImage

A template for displaying an image encircled by a configurable progress ring

Deprecated

class CLKComplicationTemplateUtilitarianSmallRingText

A template for displaying text encircled by a configurable progress ring.

Deprecated

class CLKComplicationTemplateUtilitarianSmallSquare

A template for displaying a single square image.

Deprecated

