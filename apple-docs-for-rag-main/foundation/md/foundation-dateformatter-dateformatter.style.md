

- Foundation
- DateFormatter
-  DateFormatter.Style 

Enumeration

# DateFormatter.Style

The following constants specify predefined format styles for dates and times.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum Style
```

## Overview

The format for these date and time styles is not exact because they depend on the locale, user preference settings, and the operating system version. Do not use these constants if you want an exact format.

## Topics

### Constants

case none

case short

case medium

case long

case full

case none

case short

case medium

case long

case full

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum Behavior

Constants that specify the behavior `NSDateFormatter` should exhibit.

