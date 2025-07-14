

- ClockKit
-  CLKComplicationTemplateGraphicCircularClosedGaugeView Deprecated

Class

# CLKComplicationTemplateGraphicCircularClosedGaugeView

A template for displaying a SwiftUI view inside a closed circular gauge.

ClockKitSwiftUIwatchOS 7.0–9.0Deprecated

``` source
final class CLKComplicationTemplateGraphicCircularClosedGaugeView where Label : View
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicCircular family. Figure 1 shows the layout of the view and where the template might appear on the clock face.

The following table lists the dimensions of the SwiftUI view displayed by the template. The template masks the view to a circle.

| Apple Watch Size | Width       | Height      |
|------------------|-------------|-------------|
| 40 mm            | 27 points   | 27 points   |
| 41 mm            | 28.5 points | 28.5 points |
| 44 mm            | 31 points   | 31 points   |
| 45 mm            | 32 points   | 32 points   |

## Topics

### Creating the Template

init(gaugeProvider: CLKGaugeProvider, label: Label)

Creates a new template with a closed circular gauge, and a SwiftUI view in the center.

### Accessing the Content

var gaugeProvider: CLKGaugeProvider

The gauge provider for the template.

var label: Label

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

class CLKComplicationTemplateGraphicCircularOpenGaugeView

A template for displaying a SwiftUI view, an open gauge, and text.

Deprecated

class CLKComplicationTemplateGraphicCircularStackViewText

A template for displaying a SwiftUI view and text.

Deprecated

