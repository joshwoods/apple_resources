

- ClockKit
-  CLKComplicationTemplateGraphicCircularView Deprecated

Class

# CLKComplicationTemplateGraphicCircularView

A template for displaying a circular view.

ClockKitSwiftUIwatchOS 7.0–9.0Deprecated

``` source
final class CLKComplicationTemplateGraphicCircularView where Content : View
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Mentioned in 

Building complications with SwiftUI

## Overview

This template belongs to the CLKComplicationFamily.graphicCircular family. Figure 1 shows the layout of the view and where the template might appear on the clock face.

The following table lists the dimensions of the view displayed by this template. ClockKit masks the view to a circle.

| Apple Watch Size | Width       | Height      |
|------------------|-------------|-------------|
| 40 mm            | 42 points   | 42 points   |
| 41 mm            | 44.5 points | 44.5 points |
| 44 mm            | 47 points   | 47 points   |
| 45 mm            | 50 points   | 50 points   |

## Topics

### Creating the Template

init(Content)

Creates a template that has a circular SwiftUI view.

### Accessing the Content

var content: Content

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

class CLKComplicationTemplateGraphicCircularOpenGaugeView

A template for displaying a SwiftUI view, an open gauge, and text.

Deprecated

class CLKComplicationTemplateGraphicCircularClosedGaugeView

A template for displaying a SwiftUI view inside a closed circular gauge.

Deprecated

class CLKComplicationTemplateGraphicCircularStackViewText

A template for displaying a SwiftUI view and text.

Deprecated

