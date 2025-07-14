

- Foundation
- Date
- 
  - Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
- Date.FormatStyle.Symbol.Hour
-  Date.FormatStyle.Symbol.Hour.AMPMStyle 

Structure

# Date.FormatStyle.Symbol.Hour.AMPMStyle

The format style of the string representation of the day period, before or after noon, in a date.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct AMPMStyle
```

## Overview

Possible values for this style are: omitted, narrow, abbreviated, and wide.

## Topics

### Creating AMPM Styles

static let abbreviated: Date.FormatStyle.Symbol.Hour.AMPMStyle

A type that specifies the abbreviated day period for when the locale prefers using day period with hour.

static let narrow: Date.FormatStyle.Symbol.Hour.AMPMStyle

A type that specifies the narrow day period if the locale prefers using day period with hour.

static let omitted: Date.FormatStyle.Symbol.Hour.AMPMStyle

A type that hides the day period marker.

static let wide: Date.FormatStyle.Symbol.Hour.AMPMStyle

A type that represents the wide day period if the locale prefers using day period with hour.

### Comparing AMPM Styles

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (Date, Date) -> Bool

Returns true if the two `Date` values represent the same point in time.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

