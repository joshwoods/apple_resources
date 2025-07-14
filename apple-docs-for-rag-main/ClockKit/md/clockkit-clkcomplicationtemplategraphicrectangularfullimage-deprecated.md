

- ClockKit
-  CLKComplicationTemplateGraphicRectangularFullImage Deprecated

Class

# CLKComplicationTemplateGraphicRectangularFullImage

A template for displaying a full-color image that fills the complication.

watchOS 7.0–9.0Deprecated

``` source
class CLKComplicationTemplateGraphicRectangularFullImage
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicRectangular family.

The table below lists the dimensions of the image you use in this template. Use images with a scale of `2.0` for display on Apple Watch so the point-based dimensions are half the listed size.

| Apple Watch Size | Width      | Height     |
|------------------|------------|------------|
| 40 mm            | 324 pixels | 138 pixels |
| 41 mm            | 343 pixels | 146 pixels |
| 44 mm            | 368 pixels | 156 pixels |
| 45 mm            | 386 pixels | 164 pixels |

This template supports full-color images.

Instead of providing multiple images with different resolutions, you can provide a single, scaleable PDF asset. For more information, see `Manage Assets`.

## Topics

### Creating the Template

init(imageProvider: CLKFullColorImageProvider)

Creates a template with a large rectangular image.

### Setting the Complication Data

var imageProvider: CLKFullColorImageProvider

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

### Large Images and Views

class CLKComplicationTemplateGraphicRectangularLargeImage

A template for displaying a large rectangle containing header text and an image.

Deprecated

class CLKComplicationTemplateGraphicRectangularLargeView

A template for displaying a large rectangle containing header text and a SwiftUI view.

Deprecated

class CLKComplicationTemplateGraphicRectangularFullView

A template for displaying a SwiftUI view that fills the entire template.

Deprecated

