

- ClockKit
-  CLKComplicationTemplateGraphicExtraLargeCircularOpenGaugeView Deprecated

Class

# CLKComplicationTemplateGraphicExtraLargeCircularOpenGaugeView

A template for displaying a SwiftUI view, an open gauge, and text.

ClockKitSwiftUIwatchOS 7.0–9.0Deprecated

``` source
class CLKComplicationTemplateGraphicExtraLargeCircularOpenGaugeView where Label : View
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicExtraLarge family. Figure 1 shows the layout of the complication and where it appears on the clock face.

The table below lists the dimensions of the view displayed by the template. The template masks the view to a circle.

| Apple Watch Size | Width     | Height    |
|------------------|-----------|-----------|
| 40 mm            | 31 points | 31 points |
| 41 mm            | 33 points | 33 points |
| 44 mm            | 33 points | 33 points |
| 45 mm            | 37 points | 37 points |

## Topics

### Creating the Template

init(gaugeProvider: CLKGaugeProvider, centerTextProvider: CLKTextProvider, bottomLabel: Label)

Creates a new template that has an open circular gauge, a small amount of text in the center, and a small SwiftUI view at the bottom.

### Accessing the Content

var gaugeProvider: CLKGaugeProvider

The gauge provider for the template.

var centerTextProvider: CLKTextProvider

The text provider for the center text.

var bottomLabel: Label

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

class CLKComplicationTemplateGraphicExtraLargeCircularClosedGaugeView

A template for displaying an extra-large SwiftUI view inside a closed circular gauge.

Deprecated

class CLKComplicationTemplateGraphicExtraLargeCircularStackViewText

A template for displaying a SwiftUI view and text.

Deprecated

