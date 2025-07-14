

- ClockKit
-  CLKComplicationTemplateUtilitarianSmallSquare Deprecated

Class

# CLKComplicationTemplateUtilitarianSmallSquare

A template for displaying a single square image.

watchOS 2.0–9.0Deprecated

``` source
class CLKComplicationTemplateUtilitarianSmallSquare
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.utilitarianSmall family.

The following table lists the dimensions of the image you use in this template. All dimensions are in pixels. All images must be specified as `@2x` images for display on Apple Watch, so the point-based dimensions are half the listed size.

| Apple Watch Size | Width     | Height    |
|------------------|-----------|-----------|
| 38 mm            | 40 pixels | 40 pixels |
| 40 mm            | 44 pixels | 44 pixels |
| 41 mm            | 47 pixels | 47 pixels |
| 42 mm            | 44 pixels | 44 pixels |
| 44 mm            | 50 pixels | 50 pixels |
| 45 mm            | 52 pixels | 52 pixels |

Instead of providing multiple images with different resolutions, you can provide a single, scaleable PDF asset. For more information, see `Manage Assets`.

## Topics

### Creating the Template

init(imageProvider: CLKImageProvider)

Creates a new template that has a square image.

### Setting the Complication Data

var imageProvider: CLKImageProvider

The image to display.

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

class CLKComplicationTemplateUtilitarianSmallFlat

A template for displaying an image and text in a single line.

Deprecated

class CLKComplicationTemplateUtilitarianSmallRingImage

A template for displaying an image encircled by a configurable progress ring

Deprecated

class CLKComplicationTemplateUtilitarianSmallRingText

A template for displaying text encircled by a configurable progress ring.

Deprecated

