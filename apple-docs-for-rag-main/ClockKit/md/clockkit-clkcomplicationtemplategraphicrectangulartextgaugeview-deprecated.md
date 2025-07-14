

- ClockKit
-  CLKComplicationTemplateGraphicRectangularTextGaugeView Deprecated

Class

# CLKComplicationTemplateGraphicRectangularTextGaugeView

A template for displaying a header row with a SwiftUI view and text, a second row of text, and a gauge.

ClockKitSwiftUIwatchOS 7.0–9.0Deprecated

``` source
final class CLKComplicationTemplateGraphicRectangularTextGaugeView where Label : View
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicRectangular family. Figure 1 shows the layout of the complication and where it appears on the clock face.

The following table lists the dimensions of the SwiftUI view displayed by this template.

| Apple Watch Size | Width       | Height      |
|------------------|-------------|-------------|
| 40 mm            | 12 points   | 12 points   |
| 41 mm            | 12.5 points | 12.5 points |
| 44 mm            | 13.5 points | 13.5 points |
| 45 mm            | 14.5 points | 14.5 points |

## Topics

### Creating the Template

init(headerLabel: Label, headerTextProvider: CLKTextProvider, bodyTextProvider: CLKTextProvider, gaugeProvider: CLKGaugeProvider)

Creates a new template that has a header row with a SwiftUI view and text, body text, and a gauge.

### Accessing the Content

var headerLabel: Label

The SwiftUI view displayed by the template.

var headerTextProvider: CLKTextProvider

The header text to display in the complication.

var bodyTextProvider: CLKTextProvider

The main body text to display in the complication.

var gaugeProvider: CLKGaugeProvider

The gauge to display in the complication.

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

class CLKComplicationTemplateGraphicRectangularLargeView

A template for displaying a large rectangle containing header text and a SwiftUI view.

Deprecated

class CLKComplicationTemplateGraphicRectangularFullView

A template for displaying a SwiftUI view that fills the entire template.

Deprecated

