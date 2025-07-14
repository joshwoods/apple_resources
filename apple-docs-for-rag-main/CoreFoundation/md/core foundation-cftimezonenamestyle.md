

- Core Foundation
-  CFTimeZoneNameStyle 

Enumeration

# CFTimeZoneNameStyle

Index type for constants used to specify styles of time zone names.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum CFTimeZoneNameStyle
```

## Overview

For values, see Time Zone Name Styles

## Topics

### Enumeration Cases

case daylightSaving

Specifies the daylight saving name style; for example, “Central Daylight Time” for the Central time zone.

case generic

Specifies the generic name style, which does not distinguish between daylight saving and standard time; for example, “Central Time” for the Central time zone.

case shortDaylightSaving

Specifies the short daylight saving name style; for example, “CDT” for the Central time zone.

case shortGeneric

Specifies the short generic name style, which does not distinguish between daylight saving and standard time; for example, “CT” for the Central time zone.

case shortStandard

Specifies the short standard name style; for example, “CST” for the Central time zone.

case standard

Specifies the standard name style; for example, “Central Standard Time” for the Central time zone.

### Initializers

init?(rawValue: CFIndex)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

