

- ClockKit
-  CLKComplicationTemplateGraphicExtraLargeCircularClosedGaugeView Deprecated

Class

# CLKComplicationTemplateGraphicExtraLargeCircularClosedGaugeView

A template for displaying an extra-large SwiftUI view inside a closed circular gauge.

ClockKitSwiftUIwatchOS 7.0–9.0Deprecated

``` source
final class CLKComplicationTemplateGraphicExtraLargeCircularClosedGaugeView where Label : View
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicExtraLarge family. Figure 1 shows the layout of the complication and where it appears on the clock face.

The table below lists the dimensions of the view displayed by the template. The image provider automatically masks the image to a circle.

| Apple Watch Size | Width       | Height      |
|------------------|-------------|-------------|
| 40 mm            | 77 points   | 77 points   |
| 41 mm            | 81.5 points | 81.5 points |
| 44 mm            | 87 points   | 87 points   |
| 41 mm            | 81.5 points | 81.5 points |

## Topics

### Creating the Template

init(gaugeProvider: CLKGaugeProvider, label: Label)

Creates a new template with a closed circular gauge and a SwiftUI view in the center.

### Accessing the Content

var gaugeProvider: CLKGaugeProvider

The gauge provider for the template.

var label: Label

The SwiftUI view displayed by the template.

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

### Extra large templates

class CLKComplicationTemplateGraphicExtraLargeCircularView

A template for displaying a circular SwiftUI view.

Deprecated

class CLKComplicationTemplateGraphicExtraLargeCircularOpenGaugeView

A template for displaying a SwiftUI view, an open gauge, and text.

Deprecated

class CLKComplicationTemplateGraphicExtraLargeCircularStackViewText

A template for displaying a SwiftUI view and text.

Deprecated

