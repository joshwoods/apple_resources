

- ClockKit
-  CLKComplicationTemplateGraphicExtraLargeCircularClosedGaugeImage Deprecated

Class

# CLKComplicationTemplateGraphicExtraLargeCircularClosedGaugeImage

A template for displaying an extra-large, full-color circular image inside a closed circular gauge.

watchOS 7.0–9.0Deprecated

``` source
class CLKComplicationTemplateGraphicExtraLargeCircularClosedGaugeImage
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicExtraLarge family. Figure 1 shows the layout of the complication and where it appears on the clock face.

The table below lists the dimensions of the image you use in this template. Use @2x images for display on Apple Watch so the point-based dimensions are half the listed size.

| Apple Watch Size | Width      | Height     |
|------------------|------------|------------|
| 40 mm            | 154 pixels | 154 pixels |
| 41 mm            | 163 pixels | 163 pixels |
| 44 mm            | 174 pixels | 174 pixels |
| 45 mm            | 183 pixels | 183 pixels |

This template supports full-color images. The image provider automatically masks the image to a circle.

Instead of providing multiple images with different resolutions, you can provide a single, scaleable PDF asset. For more information, see `Supporting Multiple Watch Sizes`.

## Topics

### Creating the Template

init(gaugeProvider: CLKGaugeProvider, imageProvider: CLKFullColorImageProvider)

Creates a new template with a closed circular gauge and an image in the center.

### Setting the Complication Data

var gaugeProvider: CLKGaugeProvider

The gauge to display in the complication.

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

### Open and closed gauges

class CLKComplicationTemplateGraphicExtraLargeCircularOpenGaugeImage

A template for displaying an extra-large, full-color circular image, an open gauge, and text.

Deprecated

class CLKComplicationTemplateGraphicExtraLargeCircularOpenGaugeView

A template for displaying a SwiftUI view, an open gauge, and text.

Deprecated

class CLKComplicationTemplateGraphicExtraLargeCircularOpenGaugeSimpleText

A template for displaying text inside an open gauge, with additional text at the bottom of the gauge.

Deprecated

class CLKComplicationTemplateGraphicExtraLargeCircularOpenGaugeRangeText

A template for displaying text inside an open gauge, with additional leading and trailing text.

Deprecated

class CLKComplicationTemplateGraphicExtraLargeCircularClosedGaugeView

A template for displaying an extra-large SwiftUI view inside a closed circular gauge.

Deprecated

class CLKComplicationTemplateGraphicExtraLargeCircularClosedGaugeText

A template for displaying text inside an extra-large closed circular gauge.

Deprecated

