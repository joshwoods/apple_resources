

- ClockKit
-  CLKComplicationTemplateGraphicCircularOpenGaugeSimpleText Deprecated

Class

# CLKComplicationTemplateGraphicCircularOpenGaugeSimpleText

A template for displaying text inside an open gauge, with a single piece of text for the gauge.

watchOS 5.0–9.0Deprecated

``` source
class CLKComplicationTemplateGraphicCircularOpenGaugeSimpleText
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicCircular family. Figure 1 shows the layout of the image and where the template might appear on the clock face.

## Topics

### Creating the Template

init(gaugeProvider: CLKGaugeProvider, bottomTextProvider: CLKTextProvider, centerTextProvider: CLKTextProvider)

Creates a new template with an open circular gauge, a small text element at the bottom, and a larger text element in the center.

### Setting the Complication Data

var centerTextProvider: CLKTextProvider

The text to display in the center of the gauge.

var bottomTextProvider: CLKTextProvider

The text to display at the bottom of the gauge.

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

class CLKComplicationTemplateGraphicCircularOpenGaugeImage

A template for displaying a full-color circular image, an open gauge, and text.

Deprecated

class CLKComplicationTemplateGraphicCircularOpenGaugeView

A template for displaying a SwiftUI view, an open gauge, and text.

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

