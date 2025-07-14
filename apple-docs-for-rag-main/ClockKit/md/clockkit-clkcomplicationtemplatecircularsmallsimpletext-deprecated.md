

- ClockKit
-  CLKComplicationTemplateCircularSmallSimpleText Deprecated

Class

# CLKComplicationTemplateCircularSmallSimpleText

A template for displaying a short text string.

watchOS 2.0–9.0Deprecated

``` source
class CLKComplicationTemplateCircularSmallSimpleText
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the circularSmall family.

## Topics

### Creating the Template

init(textProvider: CLKTextProvider)

Creates a new template from the provided text.

### Setting the Complication Data

var textProvider: CLKTextProvider

The text to display in the complication.

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

class CLKComplicationTemplateCircularSmallStackText

A template for displaying two text strings stacked on top of each other.

Deprecated

