

- Foundation
- DateComponentsFormatter
-  DateComponentsFormatter.UnitsStyle 

Enumeration

# DateComponentsFormatter.UnitsStyle

Constants for specifying how to represent quantities of time.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum UnitsStyle
```

## Overview

All date and time values are localized and formatted according to the current user’s language preferences.

The following table shows how the quantity of 9 hours, 41 minutes, and 30 seconds is displayed in the U.S. English locale for each style:

| Style | Displayed result |
|----|----|
| DateComponentsFormatter.UnitsStyle.spellOut | “nine hours, forty-one minutes, thirty seconds” |
| DateComponentsFormatter.UnitsStyle.full | “9 hours, 41 minutes, 30 seconds” |
| DateComponentsFormatter.UnitsStyle.short | “9 hr, 41 min, 30 sec” |
| DateComponentsFormatter.UnitsStyle.brief | “9hr 41min 30sec” |
| DateComponentsFormatter.UnitsStyle.abbreviated | “9h 41m 30s” |
| DateComponentsFormatter.UnitsStyle.positional | “9:31:30” |

## Topics

### Styles

case spellOut

A style that spells out the units and quantities of time.

case full

A style that spells out the units of time, but not the quantities.

case short

A style that uses a shortened spelling for units.

case brief

A style that uses a shortened spelling for units of time that is shorter than DateComponentsFormatter.UnitsStyle.short.

case abbreviated

A style that uses the most abbreviated spelling for units of time.

case positional

A style that uses the position of a unit of time to identify its value.

case spellOut

A style that spells out the units and quantities of time.

case full

A style that spells out the units of time, but not the quantities.

case short

A style that uses a shortened spelling for units.

case brief

A style that uses a shortened spelling for units of time that is shorter than DateComponentsFormatter.UnitsStyle.short.

case abbreviated

A style that uses the most abbreviated spelling for units of time.

case positional

A style that uses the position of a unit of time to identify its value.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

struct ZeroFormattingBehavior

Formatting constants for when values contain zeroes.

