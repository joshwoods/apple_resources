

- ClockKit
-  CLKComplicationTemplateGraphicCircularOpenGaugeView Deprecated

Class

# CLKComplicationTemplateGraphicCircularOpenGaugeView

A template for displaying a SwiftUI view, an open gauge, and text.

ClockKitSwiftUIwatchOS 7.0–9.0Deprecated

``` source
final class CLKComplicationTemplateGraphicCircularOpenGaugeView where Label : View
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicCircular family. Figure 1 shows the layout of the view and where the template might appear on the clock face.

The following table lists the dimensions of the view displayed by this template. The image provider automatically masks the image to a circle.

| Apple Watch Size | Width       | Height      |
|------------------|-------------|-------------|
| 40 mm            | 11 points   | 11 points   |
| 41 mm            | 11.5 points | 11.5 points |
| 44 mm            | 12 points   | 12 points   |
| 45 mm            | 13 points   | 13 points   |

## Topics

### Creating the Template

init(gaugeProvider: CLKGaugeProvider, centerTextProvider: CLKTextProvider, bottomLabel: Label)

Creates a new template that has an open circular gauge, a small amount of text in the center, and a small SwiftUI view at the bottom.

### Accesing the Content

var gaugeProvider: CLKGaugeProvider

The gauge provider for the template.

var centerTextProvider: CLKTextProvider

The text provider for the center text.

var bottomLabel: Label

The SwiftUI view displayed by the template.

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

### Circular templates

class CLKComplicationTemplateGraphicCircularView

A template for displaying a circular view.

Deprecated

class CLKComplicationTemplateGraphicCircularClosedGaugeView

A template for displaying a SwiftUI view inside a closed circular gauge.

Deprecated

class CLKComplicationTemplateGraphicCircularStackViewText

A template for displaying a SwiftUI view and text.

Deprecated

