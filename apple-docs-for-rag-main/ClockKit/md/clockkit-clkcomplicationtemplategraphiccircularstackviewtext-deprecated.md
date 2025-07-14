

- ClockKit
-  CLKComplicationTemplateGraphicCircularStackViewText Deprecated

Class

# CLKComplicationTemplateGraphicCircularStackViewText

A template for displaying a SwiftUI view and text.

ClockKitSwiftUIwatchOS 7.0–9.0Deprecated

``` source
final class CLKComplicationTemplateGraphicCircularStackViewText where Content : View
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicCircular family. Figure 1 shows the layout of the complication and where it appears on the clock face.

The following table lists the dimensions of the SwiftUI view displayed by the template.

| Apple Watch Size | Width     | Height    |
|------------------|-----------|-----------|
| 40 mm            | 28 points | 14 points |
| 44 mm            | 31 points | 16 points |

## Topics

### Creating the Template

init(content: Content, textProvider: CLKTextProvider)

Creates a template that has a view and a small amount of text.

### Accessing the Content

var content: Content

The SwiftUI view displayed by the template.

var textProvider: CLKTextProvider

The text to display below the view.

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

class CLKComplicationTemplateGraphicCircularClosedGaugeView

A template for displaying a SwiftUI view inside a closed circular gauge.

Deprecated

