

- ClockKit
-  CLKComplicationTemplateGraphicExtraLargeCircularStackImage Deprecated

Class

# CLKComplicationTemplateGraphicExtraLargeCircularStackImage

A template for displaying an extra-large, full-color circular image and text.

watchOS 7.0–9.0Deprecated

``` source
class CLKComplicationTemplateGraphicExtraLargeCircularStackImage
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicExtraLarge family. Figure 1 shows the layout of the complication and where it appears on the clock face.

The table below lists the dimensions of the image you use in this template. Use @2x images for display on Apple Watch so the point-based dimensions are half the listed size.

| Apple Watch Size | Width      | Height    |
|------------------|------------|-----------|
| 40 mm            | 160 pixels | 80 pixels |
| 41 mm            | 170 pixels | 84 pixels |
| 44 mm            | 174 pixels | 88 pixels |
| 45 mm            | 190 pixels | 96 pixels |

This template supports full-color images.

Instead of providing multiple images with different resolutions, you can provide a single, scaleable PDF asset. For more information, see `Supporting Multiple Watch Sizes`.

## Topics

### Creating the Template

init(line1ImageProvider: CLKFullColorImageProvider, line2TextProvider: CLKTextProvider)

Creates a template with an image and a small amount of text.

### Setting the Complication Data

var line1ImageProvider: CLKFullColorImageProvider

The image to display.

var line2TextProvider: CLKTextProvider

The text to display below the image.

## Relationships

### Inherits From

- CLKComplicationTemplateGraphicExtraLargeCircular

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

class CLKComplicationTemplateGraphicExtraLargeCircularImage

A template for displaying an extra-large, full-color circular image.

Deprecated

class CLKComplicationTemplateGraphicExtraLargeCircularView

A template for displaying a circular SwiftUI view.

Deprecated

class CLKComplicationTemplateGraphicExtraLargeCircularStackViewText

A template for displaying a SwiftUI view and text.

Deprecated

class CLKComplicationTemplateGraphicExtraLargeCircularStackText

A template for displaying two rows of text in an extra-large, circular complication.

Deprecated

