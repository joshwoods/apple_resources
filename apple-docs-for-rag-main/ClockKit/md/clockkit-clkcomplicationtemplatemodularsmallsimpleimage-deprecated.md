

- ClockKit
-  CLKComplicationTemplateModularSmallSimpleImage Deprecated

Class

# CLKComplicationTemplateModularSmallSimpleImage

A template for displaying an image.

watchOS 2.0–9.0Deprecated

``` source
class CLKComplicationTemplateModularSmallSimpleImage
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.modularSmall family.

The following table lists the dimensions of the image you use in this template. All dimensions are in pixels. All images must be specified as `@2x` images for display on Apple Watch, so the point-based dimensions are half the listed size.

| Apple Watch size | Width     | Height    |
|------------------|-----------|-----------|
| 38 mm            | 52 pixels | 52 pixels |
| 40 mm            | 58 pixels | 58 pixels |
| 41 mm            | 61 pixels | 61 pixels |
| 42 mm            | 58 pixels | 58 pixels |
| 44 mm            | 64 pixels | 64 pixels |
| 45 mm            | 69 pixels | 69 pixels |

Instead of providing multiple images with different resolutions, you can provide a single, scaleable PDF asset. For more information, see `Manage Assets`.

## Topics

### Creating the Template

init(imageProvider: CLKImageProvider)

Creates a new template from the provided image.

### Setting the Complication Data

var imageProvider: CLKImageProvider

The image to display in the complication.

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

### Image templates

class CLKComplicationTemplateModularSmallRingImage

A template for displaying an image encircled by a configurable progress ring.

Deprecated

class CLKComplicationTemplateModularSmallStackImage

A template for displaying a single image with a short line of text below it.

Deprecated

