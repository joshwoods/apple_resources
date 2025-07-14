

- ClockKit
-  CLKComplicationTemplateModularSmallRingImage Deprecated

Class

# CLKComplicationTemplateModularSmallRingImage

A template for displaying an image encircled by a configurable progress ring.

watchOS 2.0–9.0Deprecated

``` source
class CLKComplicationTemplateModularSmallRingImage
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.modularSmall family.

The following table lists the dimensions of the image you use in this template. All dimensions are in pixels. All images must be specified as `@2x` images for display on Apple Watch, so the point-based dimensions are half the listed size.

| Apple Watch Size | Width     | Height    |
|------------------|-----------|-----------|
| 38 mm            | 36 pixels | 36 pixels |
| 40 mm            | 38 pixels | 38 pixels |
| 41 mm            | 40 pixels | 40 pixels |
| 42 mm            | 38 pixels | 38 pixels |
| 44 mm            | 42 pixels | 42 pixels |
| 45 mm            | 45 pixels | 45 pixels |

Instead of providing multiple images with different resolutions, you can provide a single, scaleable PDF asset. For more information, see `Manage Assets`.

## Topics

### Creating the Template

init(imageProvider: CLKImageProvider, fillFraction: Float, ringStyle: CLKComplicationRingStyle)

Creates a new template from the provided image, fill fraction, and ring style.

### Setting the Complication Data

var imageProvider: CLKImageProvider

The image to display in the complication.

var ringStyle: CLKComplicationRingStyle

The style of the progress ring.

var fillFraction: Float

The fraction of the ring to fill.

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

class CLKComplicationTemplateModularSmallSimpleImage

A template for displaying an image.

Deprecated

class CLKComplicationTemplateModularSmallStackImage

A template for displaying a single image with a short line of text below it.

Deprecated

