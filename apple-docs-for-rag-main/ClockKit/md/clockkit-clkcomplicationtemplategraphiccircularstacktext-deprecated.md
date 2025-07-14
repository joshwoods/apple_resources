

- ClockKit
-  CLKComplicationTemplateGraphicCircularStackText Deprecated

Class

# CLKComplicationTemplateGraphicCircularStackText

A template for displaying two rows of text.

watchOS 6.0–9.0Deprecated

``` source
class CLKComplicationTemplateGraphicCircularStackText
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicCircular family.

## Topics

### Creating the Template

init(line1TextProvider: CLKTextProvider, line2TextProvider: CLKTextProvider)

Creates a new template that has two small rows of text.

### Setting the Complication Data

var line1TextProvider: CLKTextProvider

The text to display on the top row.

var line2TextProvider: CLKTextProvider

The text to display on the bottom row.

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

### Text and images

class CLKComplicationTemplateGraphicCircularImage

A template for displaying a full-color circular image.

Deprecated

class CLKComplicationTemplateGraphicCircularView

A template for displaying a circular view.

Deprecated

class CLKComplicationTemplateGraphicCircularStackImage

A template for displaying a full-color circular image and text.

Deprecated

class CLKComplicationTemplateGraphicCircularStackViewText

A template for displaying a SwiftUI view and text.

Deprecated

