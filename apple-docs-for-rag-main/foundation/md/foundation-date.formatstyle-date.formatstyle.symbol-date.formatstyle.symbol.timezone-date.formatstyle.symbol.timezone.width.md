

- Foundation
- Date
- 
  - Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
- Date.FormatStyle.Symbol.TimeZone
-  Date.FormatStyle.Symbol.TimeZone.Width 

Enumeration

# Date.FormatStyle.Symbol.TimeZone.Width

A type representing the width of a timezone in a format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum Width
```

## Overview

The possible values of a width are `short` and `long`.

## Topics

### Modifying Time Zones

case short

A short timezone representation.

case long

A long timezone representation.

### Comparing Time Zones

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

