

- ClockKit
-  CLKComplicationTemplateGraphicCornerCircularView Deprecated

Class

# CLKComplicationTemplateGraphicCornerCircularView

A template for displaying a SwiftUI view in the clock face’s corner.

ClockKitSwiftUIwatchOS 7.0–9.0Deprecated

``` source
final class CLKComplicationTemplateGraphicCornerCircularView where Content : View
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicCorner family. Figure 1 shows the layout of the view and where the template might appear on the clock face.

The following table lists the dimensions of the SwiftUI view displayed by the template. The template masks the view to a circle.

| Apple Watch Size | Width     | Height    |
|------------------|-----------|-----------|
| 40 mm            | 32 points | 32 points |
| 41 mm            | 34 points | 34 points |
| 44 mm            | 36 points | 36 points |
| 45 mm            | 38 points | 38 points |

## Topics

### Creating the Template

init(Content)

Creates a template that has a circular SwiftUI view.

### Accessing the Content

var content: Content

The SwiftUI view displayed by the template.

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

class CLKComplicationTemplateGraphicCornerGaugeView

A template for displaying a SwiftUI view and a gauge in the clock face’s corner.

Deprecated

class CLKComplicationTemplateGraphicCornerTextView

A template for displaying a SwiftUI view and text in the clock face’s corner.

Deprecated

