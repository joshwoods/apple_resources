

- ClockKit
-  CLKComplicationTemplateGraphicExtraLargeCircularView Deprecated

Class

# CLKComplicationTemplateGraphicExtraLargeCircularView

A template for displaying a circular SwiftUI view.

ClockKitSwiftUIwatchOS 7.0–9.0Deprecated

``` source
final class CLKComplicationTemplateGraphicExtraLargeCircularView where Content : View
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Mentioned in 

Building complications with SwiftUI

Adding text to a complication

## Overview

This template belongs to the CLKComplicationFamily.graphicExtraLarge family. Figure 1 shows the layout of the complication and where it appears on the clock face.

The table below lists the dimensions of the view displayed by the template. The template automatically masks the view to a circle.

| Apple Watch Size | Width      | Height     |
|------------------|------------|------------|
| 40 mm            | 120 points | 120 points |
| 41 mm            | 127 points | 127 points |
| 44 mm            | 132 points | 132 points |
| 45 mm            | 143 points | 143 points |

## Topics

### Creating the Template

init(Content)

Creates a template that has a circular view.

### Accessing the Content

var content: Content

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

class CLKComplicationTemplateGraphicExtraLargeCircularOpenGaugeView

A template for displaying a SwiftUI view, an open gauge, and text.

Deprecated

class CLKComplicationTemplateGraphicExtraLargeCircularClosedGaugeView

A template for displaying an extra-large SwiftUI view inside a closed circular gauge.

Deprecated

class CLKComplicationTemplateGraphicExtraLargeCircularStackViewText

A template for displaying a SwiftUI view and text.

Deprecated

