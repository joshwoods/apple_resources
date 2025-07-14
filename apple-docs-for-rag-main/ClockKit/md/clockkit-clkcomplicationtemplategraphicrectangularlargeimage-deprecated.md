

- ClockKit
-  CLKComplicationTemplateGraphicRectangularLargeImage Deprecated

Class

# CLKComplicationTemplateGraphicRectangularLargeImage

A template for displaying a large rectangle containing header text and an image.

watchOS 5.0–9.0Deprecated

``` source
class CLKComplicationTemplateGraphicRectangularLargeImage
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicRectangular family. Figure 1 shows the layout of the image and where the template might appear on the clock face.

The table below lists the dimensions of the image you use in this template. All dimensions are in pixels. All images must be specified as @2x images for display on Apple Watch, so the point-based dimensions are half the listed size.

| Apple Watch Size | Width      | Height     |
|------------------|------------|------------|
| 40 mm            | 300 pixels | 94 pixels  |
| 41 mm            | 318 pixels | 100 pixels |
| 44 mm            | 342 pixels | 108 pixels |
| 45 mm            | 357 pixels | 112 pixels |

This template supports full-color images. The image provider automatically masks the image to a rounded rectangle with a 8-pixel corner radius.

Instead of providing multiple images with different resolutions, you can provide a single, scaleable PDF asset. For more information, see `Supporting Multiple Watch Sizes`.

## Topics

### Creating the Template

init(textProvider: CLKTextProvider, imageProvider: CLKFullColorImageProvider)

Creates a new template with a text provider and an image provider.

### Setting the Complication Data

var textProvider: CLKTextProvider

The header text to display in the complication.

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

class CLKComplicationTemplateGraphicRectangularLargeView

A template for displaying a large rectangle containing header text and a SwiftUI view.

Deprecated

class CLKComplicationTemplateGraphicRectangularFullImage

A template for displaying a full-color image that fills the complication.

Deprecated

class CLKComplicationTemplateGraphicRectangularFullView

A template for displaying a SwiftUI view that fills the entire template.

Deprecated

