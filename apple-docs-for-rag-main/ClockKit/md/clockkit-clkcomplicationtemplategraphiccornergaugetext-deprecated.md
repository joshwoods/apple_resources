

- ClockKit
-  CLKComplicationTemplateGraphicCornerGaugeText Deprecated

Class

# CLKComplicationTemplateGraphicCornerGaugeText

A template for displaying text and a gauge in the clock face’s corner.

watchOS 5.0–9.0Deprecated

``` source
class CLKComplicationTemplateGraphicCornerGaugeText
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicCorner family. shows the layout of the image and where the template might appear on the clock face.

The system always displays the outer text as white. The gauge’s text can be multicolored.

## Topics

### Creating the Template

init(gaugeProvider: CLKGaugeProvider, outerTextProvider: CLKTextProvider)

Creates a template that has a gauge and an outer text element.

init(gaugeProvider: CLKGaugeProvider, leadingTextProvider: CLKTextProvider?, trailingTextProvider: CLKTextProvider?, outerTextProvider: CLKTextProvider)

Creates a template that has a gauge with leading and trailing text, and an outer text element.

### Setting the Complication Data

var outerTextProvider: CLKTextProvider

The outer text to display in the complication.

var gaugeProvider: CLKGaugeProvider

The gauge to display in the complication.

var leadingTextProvider: CLKTextProvider?

The text to display on the leading edge of the gague.

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

class CLKComplicationTemplateGraphicCornerGaugeImage

A template for displaying an image and a gauge in the clock face’s corner.

Deprecated

class CLKComplicationTemplateGraphicCornerGaugeView

A template for displaying a SwiftUI view and a gauge in the clock face’s corner.

Deprecated

