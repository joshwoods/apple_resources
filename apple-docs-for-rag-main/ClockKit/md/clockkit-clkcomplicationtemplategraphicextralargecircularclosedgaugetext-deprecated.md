

- ClockKit
-  CLKComplicationTemplateGraphicExtraLargeCircularClosedGaugeText Deprecated

Class

# CLKComplicationTemplateGraphicExtraLargeCircularClosedGaugeText

A template for displaying text inside an extra-large closed circular gauge.

watchOS 7.0–9.0Deprecated

``` source
class CLKComplicationTemplateGraphicExtraLargeCircularClosedGaugeText
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicExtraLarge family. Figure 1 shows the layout of the complication and where it appears on the clock face.

## Topics

### Creating the Template

init(gaugeProvider: CLKGaugeProvider, centerTextProvider: CLKTextProvider)

Creates a new template with a closed circular gauge with text in the center.

### Setting the Complication Data

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

