

- Foundation
- Date
- Date.RelativeFormatStyle
-  Date.RelativeFormatStyle.Presentation 

Structure

# Date.RelativeFormatStyle.Presentation

A type that represents the style to use when formatting relative dates, such as “1 week ago” or “last week”.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Presentation
```

## Overview

Cases include `named` and `numeric`.

## Topics

### Modifying Relative Date Style Presentations

static var named: Date.RelativeFormatStyle.Presentation

A style that uses named styles to describe relative dates, such as “yesterday”, “last week”, or “next week”.

static var numeric: Date.RelativeFormatStyle.Presentation

A style that uses a numeric style to describe relative dates, such as “1 day ago” or “in 3 weeks”.

### Comparing Relative Date Style Presentations

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

struct UnitsStyle

A type that represents the style to use when formatting the units of relative dates.

