

- ClockKit
-  CLKComplicationTemplateGraphicCircularImage Deprecated

Class

# CLKComplicationTemplateGraphicCircularImage

A template for displaying a full-color circular image.

watchOS 5.0–9.0Deprecated

``` source
class CLKComplicationTemplateGraphicCircularImage
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicCircular family. Figure 1 shows the layout of the image and where the template might appear on the clock face.

The following table lists the dimensions of the image you use in this template. All dimensions are in pixels. All images must be specified as @2x images for display on Apple Watch, so the point-based dimensions are half the listed size.

| Apple Watch Size | Width      | Height     |
|------------------|------------|------------|
| 40 mm            | 84 pixels  | 84 pixels  |
| 41 mm            | 89 pixels  | 89 pixels  |
| 44 mm            | 94 pixels  | 94 pixels  |
| 45 mm            | 100 pixels | 100 pixels |

This template supports full-color images. The image provider automatically masks the image to a circle.

Instead of providing multiple images with different resolutions, you can provide a single, scaleable PDF asset. For more information, see `Supporting Multiple Watch Sizes`.

## Topics

### Creating the Template

init(imageProvider: CLKFullColorImageProvider)

Creates a template that has a circular image.

### Setting the Complication Data

var imageProvider: CLKFullColorImageProvider

The image to display.

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

class CLKComplicationTemplateGraphicCircularView

A template for displaying a circular view.

Deprecated

class CLKComplicationTemplateGraphicCircularStackImage

A template for displaying a full-color circular image and text.

Deprecated

class CLKComplicationTemplateGraphicCircularStackViewText

A template for displaying a SwiftUI view and text.

Deprecated

class CLKComplicationTemplateGraphicCircularStackText

A template for displaying two rows of text.

Deprecated

