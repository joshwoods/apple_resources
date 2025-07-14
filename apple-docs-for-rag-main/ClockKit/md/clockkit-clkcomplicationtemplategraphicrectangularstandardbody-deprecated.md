

- ClockKit
-  CLKComplicationTemplateGraphicRectangularStandardBody Deprecated

Class

# CLKComplicationTemplateGraphicRectangularStandardBody

A template for displaying a large rectangle containing text.

watchOS 5.0–9.0Deprecated

``` source
class CLKComplicationTemplateGraphicRectangularStandardBody
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicRectangular family. Figure 1 shows the layout of the image and where the template might appear on the clock face.

The following table lists the dimensions of the image you use in this template. All dimensions are in pixels. All images must be specified as @2x images for display on Apple Watch, so the point-based dimensions are half the listed size.

| Apple Watch Size | Width     | Height    |
|------------------|-----------|-----------|
| 40 mm            | 24 pixels | 24 pixels |
| 41 mm            | 25 pixels | 25 pixels |
| 44 mm            | 27 pixels | 27 pixels |
| 45 mm            | 29 pixels | 29 pixels |

This template supports full-color images.

Instead of providing multiple images with different resolutions, you can provide a single, scaleable PDF asset. For more information, see `Supporting Multiple Watch Sizes`.

## Topics

### Creating the Template

init(headerTextProvider: CLKTextProvider, body1TextProvider: CLKTextProvider)

Creates a new template that has a row of header text and a row of body text.

init(headerTextProvider: CLKTextProvider, body1TextProvider: CLKTextProvider, body2TextProvider: CLKTextProvider?)

Creates a new template that has a row of header text and two rows of body text.

init(headerImageProvider: CLKFullColorImageProvider?, headerTextProvider: CLKTextProvider, body1TextProvider: CLKTextProvider)

Creates a new template that has a header row with an image and text, and a row of body text.

init(headerImageProvider: CLKFullColorImageProvider?, headerTextProvider: CLKTextProvider, body1TextProvider: CLKTextProvider, body2TextProvider: CLKTextProvider?)

Creates a new template that has a header row with an image and text, and two rows of body text.

### Setting the Complication Data

var headerTextProvider: CLKTextProvider

The header text to display in the complication.

var headerImageProvider: CLKFullColorImageProvider?

The header image to display.

var body1TextProvider: CLKTextProvider

The main body text to display in the complication.

var body2TextProvider: CLKTextProvider?

The secondary body text to display in the complication.

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

### Text and gauges

class CLKComplicationTemplateGraphicRectangularStandardBodyView

A template for displaying a SwiftUI label and up to three rows of text.

Deprecated

class CLKComplicationTemplateGraphicRectangularTextGauge

A template for displaying a large rectangle containing text and a gauge.

Deprecated

class CLKComplicationTemplateGraphicRectangularTextGaugeView

A template for displaying a header row with a SwiftUI view and text, a second row of text, and a gauge.

Deprecated

