

- ClockKit
-  CLKComplicationTemplateGraphicCircularClosedGaugeImage Deprecated

Class

# CLKComplicationTemplateGraphicCircularClosedGaugeImage

A template for displaying a full-color circular image and a closed circular gauge.

watchOS 5.0–9.0Deprecated

``` source
class CLKComplicationTemplateGraphicCircularClosedGaugeImage
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicCircular family. Figure 1 shows the layout of the image and where the template might appear on the clock face.

The following table lists the dimensions of the image you use in this template. All dimensions are in pixels. All images must be specified as @2x images for display on Apple Watch, so the point-based dimensions are half the listed size.

| Apple Watch Size | Width     | Height    |
|------------------|-----------|-----------|
| 40 mm            | 54 pixels | 54 pixels |
| 41 mm            | 57 pixels | 57 pixels |
| 44 mm            | 62 pixels | 62 pixels |
| 45 mm            | 64 pixels | 64 pixels |

This template supports full-color images. The image provider automatically masks the image to a circle.

Instead of providing multiple images with different resolutions, you can provide a single, scaleable PDF asset. For more information, see `Supporting Multiple Watch Sizes`.

## Topics

### Creating the Tempate

init(gaugeProvider: CLKGaugeProvider, imageProvider: CLKFullColorImageProvider)

Creates a new template with a closed circular gauge, and an image in the center.

### Setting the Complication Data

var gaugeProvider: CLKGaugeProvider

The gauge to display in the complication.

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

### Open and closed gauges

class CLKComplicationTemplateGraphicCircularOpenGaugeImage

A template for displaying a full-color circular image, an open gauge, and text.

Deprecated

class CLKComplicationTemplateGraphicCircularOpenGaugeView

A template for displaying a SwiftUI view, an open gauge, and text.

Deprecated

class CLKComplicationTemplateGraphicCircularOpenGaugeSimpleText

A template for displaying text inside an open gauge, with a single piece of text for the gauge.

Deprecated

class CLKComplicationTemplateGraphicCircularOpenGaugeRangeText

A template for displaying text inside an open gauge, with leading and trailing text for the gauge.

Deprecated

class CLKComplicationTemplateGraphicCircularClosedGaugeView

A template for displaying a SwiftUI view inside a closed circular gauge.

Deprecated

class CLKComplicationTemplateGraphicCircularClosedGaugeText

A template for displaying text inside a closed circular gauge.

Deprecated

