

- ClockKit
-  CLKComplicationTemplateExtraLargeStackText Deprecated

Class

# CLKComplicationTemplateExtraLargeStackText

A template for displaying two strings stacked one on top of the other.

watchOS 3.0–9.0Deprecated

``` source
class CLKComplicationTemplateExtraLargeStackText
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.extraLarge family.

## Topics

### Creating the Template

init(line1TextProvider: CLKTextProvider, line2TextProvider: CLKTextProvider)

Creates a new template that has two rows of text.

### Setting the Complication Data

var highlightLine2: Bool

A Boolean value indicating which line should be drawn with a highlight.

var line1TextProvider: CLKTextProvider

The text to display on the top line of the complication.

var line2TextProvider: CLKTextProvider

The text to display on the bottom line of the complication.

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

### Text templates

class CLKComplicationTemplateExtraLargeColumnsText

A template for displaying two rows and two columns of text.

Deprecated

class CLKComplicationTemplateExtraLargeRingText

A template for displaying text encircled by a configurable progress ring.

Deprecated

class CLKComplicationTemplateExtraLargeSimpleText

A template for displaying a small amount of text.

Deprecated

