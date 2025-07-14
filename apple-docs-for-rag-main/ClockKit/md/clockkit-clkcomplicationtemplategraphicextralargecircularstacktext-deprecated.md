

- ClockKit
-  CLKComplicationTemplateGraphicExtraLargeCircularStackText Deprecated

Class

# CLKComplicationTemplateGraphicExtraLargeCircularStackText

A template for displaying two rows of text in an extra-large, circular complication.

watchOS 7.0–9.0Deprecated

``` source
class CLKComplicationTemplateGraphicExtraLargeCircularStackText
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicExtraLarge family. Figure 1 shows the layout of the complication and where it appears on the clock face.

## Topics

### Creating the Template

init(line1TextProvider: CLKTextProvider, line2TextProvider: CLKTextProvider)

Creates a new template with two rows of text.

### Setting the Complication Data

var line1TextProvider: CLKTextProvider

The text to display on the top row.

var line2TextProvider: CLKTextProvider

The text to display on the bottom row.

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

### Text and images

class CLKComplicationTemplateGraphicExtraLargeCircularImage

A template for displaying an extra-large, full-color circular image.

Deprecated

class CLKComplicationTemplateGraphicExtraLargeCircularView

A template for displaying a circular SwiftUI view.

Deprecated

class CLKComplicationTemplateGraphicExtraLargeCircularStackImage

A template for displaying an extra-large, full-color circular image and text.

Deprecated

class CLKComplicationTemplateGraphicExtraLargeCircularStackViewText

A template for displaying a SwiftUI view and text.

Deprecated

