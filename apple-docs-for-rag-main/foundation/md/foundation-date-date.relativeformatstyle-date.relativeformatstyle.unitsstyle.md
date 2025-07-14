

- Foundation
- Date
- Date.RelativeFormatStyle
-  Date.RelativeFormatStyle.UnitsStyle 

Structure

# Date.RelativeFormatStyle.UnitsStyle

A type that represents the style to use when formatting the units of relative dates.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct UnitsStyle
```

## Overview

Cases include wide, narrow, abbreviated and spellOut.

## Topics

### Modifying a Relative Date Format Units Style

static var abbreviated: Date.RelativeFormatStyle.UnitsStyle

A style that uses abbreviated units, such as “2 mo. ago”.

static var narrow: Date.RelativeFormatStyle.UnitsStyle

A style that uses the shortest units, such as “2 mo. ago”.

static var spellOut: Date.RelativeFormatStyle.UnitsStyle

A style that spells out units, such as “two months ago”.

static var wide: Date.RelativeFormatStyle.UnitsStyle

A style that uses full representation of units, such as “2 months ago”.

### Comparing Relative Date Format Units Styles

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

## See Also

### Supporting Types

struct Presentation

A type that represents the style to use when formatting relative dates, such as “1 week ago” or “last week”.

