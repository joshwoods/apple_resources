

- ClockKit
-  CLKComplicationTemplateExtraLargeSimpleText Deprecated

Class

# CLKComplicationTemplateExtraLargeSimpleText

A template for displaying a small amount of text.

watchOS 3.0–9.0Deprecated

``` source
class CLKComplicationTemplateExtraLargeSimpleText
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.extraLarge family.

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

class CLKComplicationTemplateExtraLargeColumnsText

A template for displaying two rows and two columns of text.

Deprecated

class CLKComplicationTemplateExtraLargeRingText

A template for displaying text encircled by a configurable progress ring.

Deprecated

class CLKComplicationTemplateExtraLargeStackText

A template for displaying two strings stacked one on top of the other.

Deprecated

