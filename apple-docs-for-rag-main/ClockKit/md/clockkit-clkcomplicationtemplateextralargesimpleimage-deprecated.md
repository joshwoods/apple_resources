

- ClockKit
-  CLKComplicationTemplateExtraLargeSimpleImage Deprecated

Class

# CLKComplicationTemplateExtraLargeSimpleImage

A template for displaying an image.

watchOS 3.0–9.0Deprecated

``` source
class CLKComplicationTemplateExtraLargeSimpleImage
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.extraLarge family.

The following table lists the dimensions of the image you use in this template. All dimensions are in pixels. All images must be specified as `@2x` images for display on Apple Watch, so the point-based dimensions are half the listed size.

| Apple Watch Size | Width      | Height     |
|------------------|------------|------------|
| 38 mm            | 182 pixels | 182 pixels |
| 40 mm            | 203 pixels | 203 pixels |
| 41 mm            | 215 pixels | 215 pixels |
| 42 mm            | 203 pixels | 203 pixels |
| 44 mm            | 224 pixels | 224 pixels |
| 45 mm            | 242 pixels | 242 pixels |

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

class CLKComplicationTemplateExtraLargeRingImage

A template for displaying an image encircled by a configurable progress ring.

Deprecated

class CLKComplicationTemplateExtraLargeStackImage

A template for displaying a single image with a short line of text below it.

Deprecated

