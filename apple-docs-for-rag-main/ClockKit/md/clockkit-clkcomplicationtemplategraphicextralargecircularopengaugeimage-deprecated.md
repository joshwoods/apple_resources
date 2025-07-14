

- ClockKit
-  CLKComplicationTemplateGraphicExtraLargeCircularOpenGaugeImage Deprecated

Class

# CLKComplicationTemplateGraphicExtraLargeCircularOpenGaugeImage

A template for displaying an extra-large, full-color circular image, an open gauge, and text.

watchOS 7.0–9.0Deprecated

``` source
class CLKComplicationTemplateGraphicExtraLargeCircularOpenGaugeImage
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicExtraLarge family. Figure 1 shows the layout of the complication and where it appears on the clock face.

The table below lists the dimensions of the image you use in this template. Use @2x images for display on Apple Watch so the point-based dimensions are half the listed size.

| Apple Watch Size | Width     | Height    |
|------------------|-----------|-----------|
| 40 mm            | 62 pixels | 62 pixels |
| 41 mm            | 66 pixels | 66 pixels |
| 44 mm            | 66 pixels | 66 pixels |
| 45 mm            | 74 pixels | 74 pixels |

This template supports full-color images. The image provider automatically masks the image to a circle.

Instead of providing multiple images with different resolutions, you can provide a single, scaleable PDF asset. For more information, see `Supporting Multiple Watch Sizes`.

## Topics

### Creating the Template

init(gaugeProvider: CLKGaugeProvider, bottomImageProvider: CLKFullColorImageProvider, centerTextProvider: CLKTextProvider)

Creates a new template with an open circular gauge, an image at the bottom, and text in the center.

### Setting the Complication Data

var bottomImageProvider: CLKFullColorImageProvider

The image to display at the bottom of the gauge.

var centerTextProvider: CLKTextProvider

The text to display in the center of the gauge.

var gaugeProvider: CLKGaugeProvider

The gauge to display in the complication.

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

### Open and closed gauges

class CLKComplicationTemplateGraphicExtraLargeCircularOpenGaugeView

A template for displaying a SwiftUI view, an open gauge, and text.

Deprecated

class CLKComplicationTemplateGraphicExtraLargeCircularOpenGaugeSimpleText

A template for displaying text inside an open gauge, with additional text at the bottom of the gauge.

Deprecated

class CLKComplicationTemplateGraphicExtraLargeCircularOpenGaugeRangeText

A template for displaying text inside an open gauge, with additional leading and trailing text.

Deprecated

class CLKComplicationTemplateGraphicExtraLargeCircularClosedGaugeImage

A template for displaying an extra-large, full-color circular image inside a closed circular gauge.

Deprecated

class CLKComplicationTemplateGraphicExtraLargeCircularClosedGaugeView

A template for displaying an extra-large SwiftUI view inside a closed circular gauge.

Deprecated

class CLKComplicationTemplateGraphicExtraLargeCircularClosedGaugeText

A template for displaying text inside an extra-large closed circular gauge.

Deprecated

