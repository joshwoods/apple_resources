

- ClockKit
-  CLKComplicationTemplateGraphicCircularOpenGaugeImage Deprecated

Class

# CLKComplicationTemplateGraphicCircularOpenGaugeImage

A template for displaying a full-color circular image, an open gauge, and text.

watchOS 5.0–9.0Deprecated

``` source
class CLKComplicationTemplateGraphicCircularOpenGaugeImage
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicCircular family. Figure 1 shows the layout of the image and where the template might appear on the clock face.

The following table lists the dimensions of the image you use in this template. All dimensions are in pixels. All images must be specified as @2x images for display on Apple Watch, so the point-based dimensions are half the listed size.

| Apple Watch Size | Width     | Height    |
|------------------|-----------|-----------|
| 40 mm            | 22 pixels | 22 pixels |
| 41 mm            | 23 pixels | 23 pixels |
| 44 mm            | 24 pixels | 24 pixels |
| 45 mm            | 26 pixels | 26 pixels |

This template supports full-color images. The image provider automatically masks the image to a circle.

Instead of providing multiple images with different resolutions, you can provide a single, scaleable PDF asset. For more information, see `Supporting Multiple Watch Sizes`.

## Topics

### Creating the Template

init(gaugeProvider: CLKGaugeProvider, bottomImageProvider: CLKFullColorImageProvider, centerTextProvider: CLKTextProvider)

Creates a new template that has an open circular gauge, a small image at the bottom, and a small amount of text in the center.

### Setting the Complication Data

var bottomImageProvider: CLKFullColorImageProvider

The image to display at the bottom of the gauge.

var centerTextProvider: CLKTextProvider

The text to display in the center of the gauge.

var gaugeProvider: CLKGaugeProvider

The gauge to display in the complication.

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

class CLKComplicationTemplateGraphicCircularOpenGaugeView

A template for displaying a SwiftUI view, an open gauge, and text.

Deprecated

class CLKComplicationTemplateGraphicCircularOpenGaugeSimpleText

A template for displaying text inside an open gauge, with a single piece of text for the gauge.

Deprecated

class CLKComplicationTemplateGraphicCircularOpenGaugeRangeText

A template for displaying text inside an open gauge, with leading and trailing text for the gauge.

Deprecated

class CLKComplicationTemplateGraphicCircularClosedGaugeImage

A template for displaying a full-color circular image and a closed circular gauge.

Deprecated

class CLKComplicationTemplateGraphicCircularClosedGaugeView

A template for displaying a SwiftUI view inside a closed circular gauge.

Deprecated

class CLKComplicationTemplateGraphicCircularClosedGaugeText

A template for displaying text inside a closed circular gauge.

Deprecated

