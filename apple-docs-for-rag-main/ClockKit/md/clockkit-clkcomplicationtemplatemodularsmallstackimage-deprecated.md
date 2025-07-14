

- ClockKit
-  CLKComplicationTemplateModularSmallStackImage Deprecated

Class

# CLKComplicationTemplateModularSmallStackImage

A template for displaying a single image with a short line of text below it.

watchOS 2.0–9.0Deprecated

``` source
class CLKComplicationTemplateModularSmallStackImage
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.modularSmall family.

The following table lists the dimensions of the image you use in this template. All dimensions are in pixels. All images must be specified as `@2x` images for display on Apple Watch, so the point-based dimensions are half the listed size.

| Apple Watch Size | Width | Height |
|----|----|----|
| 38 mm | 52 pixels maximum  (You may specify images with a smaller width.) | 28 pixels |
| 40 mm | 58 pixels maximum  (You may specify images with a smaller width.) | 30 pixels |
| 41 mm | 61 pixels  (You may specify images with a smaller width.) | 32 pixels |
| 42 mm | 58 pixels maximum  (You may specify images with a smaller width.) | 30 pixels |
| 44 mm | 64 pixels maximum  (You may specify images with a smaller width.) | 34 pixels |
| 45 mm | 69 pixels  (You may specify images with a smaller width.) | 36 pixels |

Instead of providing multiple images with different resolutions, you can provide a single, scaleable PDF asset. For more information, see `Manage Assets`.

## Topics

### Creating the Template

init(line1ImageProvider: CLKImageProvider, line2TextProvider: CLKTextProvider)

Creates a new template from the provided image and text.

### Setting the Complication Data

var line1ImageProvider: CLKImageProvider

The image to display on the top line of the complication.

var line2TextProvider: CLKTextProvider

The text to display on the bottom line of the complication.

var highlightLine2: Bool

A Boolean value indicating which line should be drawn with a highlight.

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

class CLKComplicationTemplateModularSmallSimpleImage

A template for displaying an image.

Deprecated

