

- ClockKit
-  CLKComplicationTemplateGraphicCornerTextImage Deprecated

Class

# CLKComplicationTemplateGraphicCornerTextImage

A template for displaying an image and text in the clock face’s corner.

watchOS 5.0–9.0Deprecated

``` source
class CLKComplicationTemplateGraphicCornerTextImage
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicCorner family. Figure 1 shows the layout of the image and where the template might appear on the clock face.

The following table lists the dimensions of the image you use in this template. All dimensions are in pixels. All images must be specified as @2x images for display on Apple Watch, so the point-based dimensions are half the listed size.

| Apple Watch Size | Width     | Height    |
|------------------|-----------|-----------|
| 40 mm            | 40 pixels | 40 pixels |
| 41 mm            | 42 pixels | 42 pixels |
| 44 mm            | 44 pixels | 44 pixels |
| 45 mm            | 48 pixels | 48 pixels |

This template supports full-color images. The image provider automatically masks the image to a circle.

Instead of providing multiple images with different resolutions, you can provide a single, scaleable PDF asset. For more information, see `Supporting Multiple Watch Sizes`.

## Topics

### Creating the Template

init(textProvider: CLKTextProvider, imageProvider: CLKFullColorImageProvider)

Creates a template with a line of text and an image.

### Setting the Complication Data

var imageProvider: CLKFullColorImageProvider

The image to display.

var textProvider: CLKTextProvider

The text to display in the complication.

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

### Text and image

class CLKComplicationTemplateGraphicCornerCircularImage

A template for displaying an image in the clock face’s corner.

Deprecated

class CLKComplicationTemplateGraphicCornerCircularView

A template for displaying a SwiftUI view in the clock face’s corner.

Deprecated

class CLKComplicationTemplateGraphicCornerStackText

A template for displaying stacked text in the clock face’s corner.

Deprecated

class CLKComplicationTemplateGraphicCornerTextView

A template for displaying a SwiftUI view and text in the clock face’s corner.

Deprecated

