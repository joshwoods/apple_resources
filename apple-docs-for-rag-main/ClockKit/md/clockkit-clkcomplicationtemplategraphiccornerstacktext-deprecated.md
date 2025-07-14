

- ClockKit
-  CLKComplicationTemplateGraphicCornerStackText Deprecated

Class

# CLKComplicationTemplateGraphicCornerStackText

A template for displaying stacked text in the clock face’s corner.

watchOS 5.0–9.0Deprecated

``` source
class CLKComplicationTemplateGraphicCornerStackText
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.graphicCorner family. shows the layout of the image and where the template might appear on the clock face.

The system always displays the outer text as white. The inner text can be multicolored.

## Topics

### Creating the Template

init(innerTextProvider: CLKTextProvider, outerTextProvider: CLKTextProvider)

Creates a template that has an inner line of text and an outer text element.

### Setting the Complication Data

var outerTextProvider: CLKTextProvider

The outer text to display in the complication.

var innerTextProvider: CLKTextProvider

The inner text to display in the complication.

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

### Text and image

class CLKComplicationTemplateGraphicCornerCircularImage

A template for displaying an image in the clock face’s corner.

Deprecated

class CLKComplicationTemplateGraphicCornerCircularView

A template for displaying a SwiftUI view in the clock face’s corner.

Deprecated

class CLKComplicationTemplateGraphicCornerTextImage

A template for displaying an image and text in the clock face’s corner.

Deprecated

class CLKComplicationTemplateGraphicCornerTextView

A template for displaying a SwiftUI view and text in the clock face’s corner.

Deprecated

