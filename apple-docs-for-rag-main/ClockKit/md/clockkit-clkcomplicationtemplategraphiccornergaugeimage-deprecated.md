

- ClockKit
-  CLKComplicationTemplateGraphicCornerGaugeImage Deprecated

Class

# CLKComplicationTemplateGraphicCornerGaugeImage

A template for displaying an image and a gauge in the clock face’s corner.

watchOS 5.0–9.0Deprecated

``` source
class CLKComplicationTemplateGraphicCornerGaugeImage
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

init(gaugeProvider: CLKGaugeProvider, imageProvider: CLKFullColorImageProvider)

Creates a new template that has a gauge and an image.

init(gaugeProvider: CLKGaugeProvider, leadingTextProvider: CLKTextProvider?, trailingTextProvider: CLKTextProvider?, imageProvider: CLKFullColorImageProvider)

Creates a new template that has a gauge with leading and trailing text and an image.

### Setting the Complication Data

var imageProvider: CLKFullColorImageProvider

The image to display.

var gaugeProvider: CLKGaugeProvider

The gauge to display in the complication.

var leadingTextProvider: CLKTextProvider?

The text to display on the leading edge of the gauge.

var trailingTextProvider: CLKTextProvider?

The text to display on the trailing edge of the gauge.

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

### Gauges

class CLKComplicationTemplateGraphicCornerGaugeView

A template for displaying a SwiftUI view and a gauge in the clock face’s corner.

Deprecated

class CLKComplicationTemplateGraphicCornerGaugeText

A template for displaying text and a gauge in the clock face’s corner.

Deprecated

