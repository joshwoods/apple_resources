

- ClockKit
-  CLKComplicationTemplateGraphicExtraLargeCircularImage Deprecated

Class

# CLKComplicationTemplateGraphicExtraLargeCircularImage

A template for displaying an extra-large, full-color circular image.

watchOS 7.0–9.0Deprecated

``` source
class CLKComplicationTemplateGraphicExtraLargeCircularImage
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicExtraLarge family. Figure 1 shows the layout of the complication and where it appears on the clock face.

The table below lists the dimensions of the image you use in this template. Use @2x images for display on Apple Watch so the point-based dimensions are half the listed size.

| Apple Watch Size | Width      | Height     |
|------------------|------------|------------|
| 40 mm            | 240 pixels | 240 pixels |
| 41 mm            | 254 pixels | 254 pixels |
| 44 mm            | 264 pixels | 264 pixels |
| 45 mm            | 286 pixels | 286 pixels |

This template supports full-color images. The image provider automatically masks the image to a circle.

Instead of providing multiple images with different resolutions, you can provide a single, scaleable PDF asset. For more information, see `Supporting Multiple Watch Sizes`.

## Topics

### Creating the Template

init(imageProvider: CLKFullColorImageProvider)

Creates a template with a circular image.

### Setting the Complication Data

var imageProvider: CLKFullColorImageProvider

The image to display.

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

class CLKComplicationTemplateGraphicExtraLargeCircularView

A template for displaying a circular SwiftUI view.

Deprecated

class CLKComplicationTemplateGraphicExtraLargeCircularStackImage

A template for displaying an extra-large, full-color circular image and text.

Deprecated

class CLKComplicationTemplateGraphicExtraLargeCircularStackViewText

A template for displaying a SwiftUI view and text.

Deprecated

class CLKComplicationTemplateGraphicExtraLargeCircularStackText

A template for displaying two rows of text in an extra-large, circular complication.

Deprecated

