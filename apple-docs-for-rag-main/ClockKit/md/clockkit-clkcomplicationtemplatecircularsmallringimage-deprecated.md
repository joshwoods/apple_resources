

- ClockKit
-  CLKComplicationTemplateCircularSmallRingImage Deprecated

Class

# CLKComplicationTemplateCircularSmallRingImage

A template for displaying a single image surrounded by a configurable progress ring.

watchOS 2.0–9.0Deprecated

``` source
class CLKComplicationTemplateCircularSmallRingImage
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.circularSmall family.

The following table lists the dimensions of the image you use in this template. All dimensions are in pixels. All images must be specified as `@2x` images for display on Apple Watch, so the point-based dimensions are half the listed size.

| Apple Watch Size | Width     | Height    |
|------------------|-----------|-----------|
| 38 mm            | 40 pixels | 40 pixels |
| 40 mm            | 44 pixels | 44 pixels |
| 41 mm            | 47 pixels | 47 pixels |
| 42 mm            | 44 pixels | 44 pixels |
| 44 mm            | 48 pixels | 48 pixels |
| 45 mm            | 52 pixels | 52 pixels |

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

class CLKComplicationTemplateCircularSmallSimpleImage

A template for displaying a single image.

Deprecated

class CLKComplicationTemplateCircularSmallStackImage

A template for displaying an image with a line of text below it.

Deprecated

