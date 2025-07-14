

- ClockKit
-  CLKComplicationTemplateExtraLargeStackImage Deprecated

Class

# CLKComplicationTemplateExtraLargeStackImage

A template for displaying a single image with a short line of text below it.

watchOS 3.0–9.0Deprecated

``` source
class CLKComplicationTemplateExtraLargeStackImage
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.extraLarge family.

The following table lists the dimensions of the image you use in this template. All dimensions are in pixels. All images must be specified as `@2x` images for display on Apple Watch, so the point-based dimensions are half the listed size.

| Apple Watch Size | Width | Height |
|----|----|----|
| 38 mm | 156 pixels maximum  (You may specify images with a smaller width.) | 84 pixels |
| 40 mm | 174 pixels maximum  (You may specify images with a smaller width.) | 90 pixels |
| 41 mm | 192 pixels maximum  (You may specify images with a smaller width.) | 95 pixels |
| 42 mm | 174 pixels maximum  (You may specify images with a smaller width.) | 90 pixels |
| 44 mm | 192 pixels maximum  (You may specify images with a smaller width.) | 102 pixels |
| 45 mm | 207 pixels  (You may specify images with a smaller width.) | 107 pixels |

Instead of providing multiple images with different resolutions, you can provide a single, scaleable PDF asset. For more information, see `Manage Assets`.

## Topics

### Creating the Template

init(line1ImageProvider: CLKImageProvider, line2TextProvider: CLKTextProvider)

Creates a new template from the provided image and text.

### Setting the Complication Data

var highlightLine2: Bool

A Boolean value indicating which line should be drawn with a highlight.

var line1ImageProvider: CLKImageProvider

The image to display on the top line of the complication.

var line2TextProvider: CLKTextProvider

The text to display on the bottom line of the complication.

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

class CLKComplicationTemplateExtraLargeSimpleImage

A template for displaying an image.

Deprecated

