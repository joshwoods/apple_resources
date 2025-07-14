

- ClockKit
-  CLKComplicationTemplateGraphicRectangularFullView Deprecated

Class

# CLKComplicationTemplateGraphicRectangularFullView

A template for displaying a SwiftUI view that fills the entire template.

ClockKitSwiftUIwatchOS 7.0–9.0Deprecated

``` source
final class CLKComplicationTemplateGraphicRectangularFullView where Content : View
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Mentioned in 

Building complications with SwiftUI

## Overview

This template belongs to the CLKComplicationFamily.graphicRectangular family. Figure 1 shows the layout of the complication and where it appears on the clock face.

The following table lists the dimensions of the view displayed by this template. The template automatically masks the view to a rounded rectangle with a 8-pixel corner radius. By default, the template also provides a safe area inset to help you avoid clipping your content. Use the edgesIgnoringSafeArea(_:) modifier if you need to fill the complication to the edges.

| Apple Watch Size        | Width        | Height    |
|-------------------------|--------------|-----------|
| 40 mm (safe area inset) | 150 points   | 57 points |
| 40 mm (full view)       | 162 points   | 69 points |
| 41 mm (safe area inset) | 158.5 points | 60 points |
| 41 mm (full view)       | 171.5 points | 73 points |
| 44 mm (safe area inset) | 171 points   | 65 points |
| 44 mm (full view)       | 184 points   | 78 points |
| 45 mm (safe area inset) | 179 points   | 68 points |
| 45 mm (full view)       | 193 points   | 82 points |

## Topics

### Creating the Template

init(Content)

Creates a template that has a circular image.

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

### Rectangular templates

class CLKComplicationTemplateGraphicRectangularStandardBodyView

A template for displaying a SwiftUI label and up to three rows of text.

Deprecated

class CLKComplicationTemplateGraphicRectangularTextGaugeView

A template for displaying a header row with a SwiftUI view and text, a second row of text, and a gauge.

Deprecated

class CLKComplicationTemplateGraphicRectangularLargeView

A template for displaying a large rectangle containing header text and a SwiftUI view.

Deprecated

