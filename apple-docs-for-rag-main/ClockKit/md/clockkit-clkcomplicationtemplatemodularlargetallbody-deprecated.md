

- ClockKit
-  CLKComplicationTemplateModularLargeTallBody Deprecated

Class

# CLKComplicationTemplateModularLargeTallBody

A template for displaying a header row and row of tall body text.

watchOS 2.0–9.0Deprecated

``` source
class CLKComplicationTemplateModularLargeTallBody
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

This template belongs to the CLKComplicationFamily.modularLarge family.

## Topics

### Creating the Template

init(headerTextProvider: CLKTextProvider, bodyTextProvider: CLKTextProvider)

Creates a template that has a header and a row of tall body text.

### Setting the Complication Data

var headerTextProvider: CLKTextProvider

The text to display in the header line.

var bodyTextProvider: CLKTextProvider

The text to display in the body line.

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

### Body templates

class CLKComplicationTemplateModularLargeStandardBody

A template for displaying a header row and two lines of text.

Deprecated

