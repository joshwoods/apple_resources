

- ClockKit
-  CLKComplicationTemplateGraphicCircularStackImage Deprecated

Class

# CLKComplicationTemplateGraphicCircularStackImage

A template for displaying a full-color circular image and text.

watchOS 6.0–9.0Deprecated

``` source
class CLKComplicationTemplateGraphicCircularStackImage
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicCircular family.

The following table lists the dimensions of the image you use in this template. All dimensions are in pixels. All images must be specified as @2x images for display on Apple Watch, so the point-based dimensions are half the listed size.

| Apple Watch Size | Width     | Height    |
|------------------|-----------|-----------|
| 40 mm            | 56 pixels | 28 pixels |
| 41 mm            | 59 pixels | 30 pixels |
| 44 mm            | 62 pixels | 32 pixels |
| 45 mm            | 67 pixels | 33 pixels |

This template supports full-color images.

Instead of providing multiple images with different resolutions, you can provide a single, scaleable PDF asset. For more information, see `Supporting Multiple Watch Sizes`.

## Topics

### Creating the Template

init(line1ImageProvider: CLKFullColorImageProvider, line2TextProvider: CLKTextProvider)

Creates a template that has an image and a small amount of text.

### Setting the Complicaiton Data

var line1ImageProvider: CLKFullColorImageProvider

The image to display.

var line2TextProvider: CLKTextProvider

The text to display below the image.

## Relationships

### Inherits From

- CLKComplicationTemplateGraphicCircular

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Text and images

class CLKComplicationTemplateGraphicCircularImage

A template for displaying a full-color circular image.

Deprecated

class CLKComplicationTemplateGraphicCircularView

A template for displaying a circular view.

Deprecated

class CLKComplicationTemplateGraphicCircularStackViewText

A template for displaying a SwiftUI view and text.

Deprecated

class CLKComplicationTemplateGraphicCircularStackText

A template for displaying two rows of text.

Deprecated

