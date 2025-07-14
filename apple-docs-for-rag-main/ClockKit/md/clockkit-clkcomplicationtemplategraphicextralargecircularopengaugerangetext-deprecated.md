

- ClockKit
-  CLKComplicationTemplateGraphicExtraLargeCircularOpenGaugeRangeText Deprecated

Class

# CLKComplicationTemplateGraphicExtraLargeCircularOpenGaugeRangeText

A template for displaying text inside an open gauge, with additional leading and trailing text.

watchOS 7.0–9.0Deprecated

``` source
class CLKComplicationTemplateGraphicExtraLargeCircularOpenGaugeRangeText
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicExtraLarge family. Figure 1 shows the layout of the complication and where it appears on the clock face.

## Topics

### Creating the Template

init(gaugeProvider: CLKGaugeProvider, leadingTextProvider: CLKTextProvider, trailingTextProvider: CLKTextProvider, centerTextProvider: CLKTextProvider)

Creates a new template that has an open, circular gauge with leading and trailing text, and a central text element.

### Setting the Complication Data

var centerTextProvider: CLKTextProvider

The text to display in the center of the gauge.

var gaugeProvider: CLKGaugeProvider

The gauge to display in the complication.

var leadingTextProvider: CLKTextProvider

The text to display on the leading edge of the gauge.

var trailingTextProvider: CLKTextProvider

The text to display on the trailing edge of the gauge.

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

class CLKComplicationTemplateGraphicExtraLargeCircularClosedGaugeImage

A template for displaying an extra-large, full-color circular image inside a closed circular gauge.

Deprecated

class CLKComplicationTemplateGraphicExtraLargeCircularClosedGaugeView

A template for displaying an extra-large SwiftUI view inside a closed circular gauge.

Deprecated

class CLKComplicationTemplateGraphicExtraLargeCircularClosedGaugeText

A template for displaying text inside an extra-large closed circular gauge.

Deprecated

