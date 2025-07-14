

- ClockKit
-  CLKSimpleTextProvider Deprecated

Class

# CLKSimpleTextProvider

A single line of text to display in your complication interface.

watchOS 2.0–9.0Deprecated

``` source
class CLKSimpleTextProvider
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Mentioned in 

Creating a timeline entry

## Overview

Use a simple text provider to specify strings for your complications. The simple text object handles the formatting of that string in your complication, which may include tinting it to match the color of the clock face.

When creating a simple text provider, you can specify both a long version and a short version of your text. Providing both strings gives you more control over the text displayed by your complication. When the long string doesn’t fit in the available space, the text provider tries to display the value in the shortText property instead. If the shorter version is still too long, it displays a truncated version of the longer text.

## Topics

### Creating a Text Provider

convenience init(text: String)

Creates and returns a text provider with the specified long form text.

convenience init(text: String, shortText: String?)

Creates and returns a text provider with both long and short versions of the text.

convenience init(text: String, shortText: String?, accessibilityLabel: String?)

Creates and returns a text provider with the text strings and an accessible string.

### Getting the Text

var text: String

The long version of text that you want to display.

var shortText: String?

A shorter version of the text.

## Relationships

### Inherits From

- CLKTextProvider

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Text providers

class CLKDateTextProvider

A formatted string that conveys a date without any time information.

Deprecated

class CLKRelativeDateTextProvider

A formatted string that conveys the difference in time between the current date and a date that you specify.

Deprecated

class CLKTimeIntervalTextProvider

A formatted time range.

Deprecated

class CLKTimeTextProvider

A formatted time value.

Deprecated

class CLKTextProvider

The common behavior for displaying text-based data in a complication.

Deprecated

