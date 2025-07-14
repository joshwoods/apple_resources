

- ClockKit
-  CLKComplicationTemplateGraphicExtraLargeCircularStackViewText Deprecated

Class

# CLKComplicationTemplateGraphicExtraLargeCircularStackViewText

A template for displaying a SwiftUI view and text.

ClockKitSwiftUIwatchOS 7.0–9.0Deprecated

``` source
final class CLKComplicationTemplateGraphicExtraLargeCircularStackViewText where Content : View
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicExtraLarge family. Figure 1 shows the layout of the complication and where it appears on the clock face.

The table below lists the dimensions of the view displayed by the template.

| Apple Watch Size | Width       | Height    |
|------------------|-------------|-----------|
| 40 mm            | 40 points   | 20 points |
| 44 mm            | 43.5 points | 22 points |

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

class CLKComplicationTemplateGraphicExtraLargeCircularClosedGaugeView

A template for displaying an extra-large SwiftUI view inside a closed circular gauge.

Deprecated

