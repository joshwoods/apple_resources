

- ClockKit
-  CLKComplicationTemplateGraphicExtraLargeCircularOpenGaugeSimpleText Deprecated

Class

# CLKComplicationTemplateGraphicExtraLargeCircularOpenGaugeSimpleText

A template for displaying text inside an open gauge, with additional text at the bottom of the gauge.

watchOS 7.0–9.0Deprecated

``` source
class CLKComplicationTemplateGraphicExtraLargeCircularOpenGaugeSimpleText
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicExtraLarge family. Figure 1 shows the layout of the complication and where it appears on the clock face.

## Topics

### Creating the Template

init(gaugeProvider: CLKGaugeProvider, bottomTextProvider: CLKTextProvider, centerTextProvider: CLKTextProvider)

Creates a new template with an open circular gauge, a small text element at the bottom, and a larger text element in the center.

### Setting the Complication Data

var bottomTextProvider: CLKTextProvider

The text to display at the bottom of the gauge.

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

class CLKComplicationTemplateGraphicExtraLargeCircularOpenGaugeImage

A template for displaying an extra-large, full-color circular image, an open gauge, and text.

Deprecated

class CLKComplicationTemplateGraphicExtraLargeCircularOpenGaugeView

A template for displaying a SwiftUI view, an open gauge, and text.

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

