

- Foundation
- Date
- 
  - Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
- Date.FormatStyle.Symbol.DayPeriod
-  Date.FormatStyle.Symbol.DayPeriod.Width 

Enumeration

# Date.FormatStyle.Symbol.DayPeriod.Width

A type representing the width of a day period in a format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum Width
```

## Overview

The possible values of a width are `abbreviated`, `narrow`, and `wide`.

## Topics

### Modifying a Day Period Width

case abbreviated

A shortened day period width representation.

case narrow

The shortest day period width representation.

case wide

A full day period width representation.

### Comparing Day Period Widths

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (Date, Date) -> Bool

Returns true if the two `Date` values represent the same point in time.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

