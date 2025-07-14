

- ClockKit
-  CLKComplicationTemplateGraphicRectangularLargeView Deprecated

Class

# CLKComplicationTemplateGraphicRectangularLargeView

A template for displaying a large rectangle containing header text and a SwiftUI view.

ClockKitSwiftUIwatchOS 7.0–9.0Deprecated

``` source
final class CLKComplicationTemplateGraphicRectangularLargeView where Content : View
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicRectangular family. Figure 1 shows the layout of the complication and where it appears on the clock face.

The following table lists the dimensions of the view displayed by this template. The template automatically masks the view to a rounded rectangle with a 8-pixel corner radius.

| Apple Watch Size | Width        | Height    |
|------------------|--------------|-----------|
| 40 mm            | 150 points   | 47 points |
| 41 mm            | 159 points   | 50 points |
| 44 mm            | 171 points   | 54 points |
| 45 mm            | 178.5 points | 56 points |

## Topics

### Creating the Template

init(headerTextProvider: CLKTextProvider, content: Content)

Creates a new template with a text provider and a SwiftUI view.

### Accessing the Content

var headerTextProvider: CLKTextProvider

The text provider for a row of text.

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

class CLKComplicationTemplateGraphicRectangularFullView

A template for displaying a SwiftUI view that fills the entire template.

Deprecated

