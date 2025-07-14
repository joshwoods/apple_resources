

- ClockKit
-  CLKComplicationTemplateCircularSmallStackText Deprecated

Class

# CLKComplicationTemplateCircularSmallStackText

A template for displaying two text strings stacked on top of each other.

watchOS 2.0–9.0Deprecated

``` source
class CLKComplicationTemplateCircularSmallStackText
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.circularSmall family.

## Topics

### Creating the Template

init(line1TextProvider: CLKTextProvider, line2TextProvider: CLKTextProvider)

Creates a new template that has two lines of text.

### Setting the Complication Data

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

class CLKComplicationTemplateCircularSmallRingText

A template for displaying a short text string encircled by a configurable progress ring.

Deprecated

class CLKComplicationTemplateCircularSmallSimpleText

A template for displaying a short text string.

Deprecated

