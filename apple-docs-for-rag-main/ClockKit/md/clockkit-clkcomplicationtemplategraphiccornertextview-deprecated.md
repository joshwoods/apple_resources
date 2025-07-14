

- ClockKit
-  CLKComplicationTemplateGraphicCornerTextView Deprecated

Class

# CLKComplicationTemplateGraphicCornerTextView

A template for displaying a SwiftUI view and text in the clock face’s corner.

ClockKitSwiftUIwatchOS 7.0–9.0Deprecated

``` source
final class CLKComplicationTemplateGraphicCornerTextView where Label : View
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicCorner family. shows the layout of the view and where the template might appear on the clock face.

The following table lists the dimensions of the view displayed by the template. The template masks the view to a circle.

| Apple Watch Size | Width     | Height    |
|------------------|-----------|-----------|
| 40 mm            | 20 points | 20 points |
| 41 mm            | 21 points | 21 points |
| 44 mm            | 22 points | 22 points |
| 45 mm            | 24 points | 24 points |

## Topics

### Creating the Template

init(textProvider: CLKTextProvider, label: Label)

Creates a template with a line of text and a SwiftUI view.

### Accessing the Content

var textProvider: CLKTextProvider

The text provider for the text.

var label: Label

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

class CLKComplicationTemplateGraphicCornerCircularView

A template for displaying a SwiftUI view in the clock face’s corner.

Deprecated

class CLKComplicationTemplateGraphicCornerGaugeView

A template for displaying a SwiftUI view and a gauge in the clock face’s corner.

Deprecated

