

- ClockKit
-  CLKComplicationTemplateGraphicCornerGaugeView Deprecated

Class

# CLKComplicationTemplateGraphicCornerGaugeView

A template for displaying a SwiftUI view and a gauge in the clock face’s corner.

ClockKitSwiftUIwatchOS 7.0–9.0Deprecated

``` source
final class CLKComplicationTemplateGraphicCornerGaugeView where Label : View
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicCorner family. Figure 1 shows the layout of the view and where the template might appear on the clock face.

The following table lists the dimensions of the view displayed by this template. ClockKIt masks the view to a circle.

| Apple Watch Size | Width     | Height    |
|------------------|-----------|-----------|
| 40 mm            | 20 points | 20 points |
| 41 mm            | 21 points | 21 points |
| 44 mm            | 22 points | 22 points |
| 45 mm            | 24 points | 24 points |

## Topics

### Creating the Template

init(gaugeProvider: CLKGaugeProvider, leadingTextProvider: CLKTextProvider?, trailingTextProvider: CLKTextProvider?, label: Label)

Creates a new template with the provided gauge and view.

### Accessing the Content

var label: Label

The SwiftUI view displayed by the template.

var gaugeProvider: CLKGaugeProvider

The gauge to display in the complication.

var leadingTextProvider: CLKTextProvider?

The text provider for the gauge’s leading text.

var trailingTextProvider: CLKTextProvider?

The text provider for the gauge’s trailing text.

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

### Corner templates

class CLKComplicationTemplateGraphicCornerCircularView

A template for displaying a SwiftUI view in the clock face’s corner.

Deprecated

class CLKComplicationTemplateGraphicCornerTextView

A template for displaying a SwiftUI view and text in the clock face’s corner.

Deprecated

