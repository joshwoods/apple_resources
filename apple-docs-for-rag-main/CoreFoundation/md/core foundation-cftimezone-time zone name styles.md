

- Core Foundation
- CFTimeZone
-  Time Zone Name Styles 

API Collection

# Time Zone Name Styles

Constants to specify styles for time zone names.

## Overview

These constants are used with the function CFTimeZoneCopyLocalizedName(_:_:_:).

## Topics

### Constants

case standard

Specifies the standard name style; for example, “Central Standard Time” for the Central time zone.

case shortStandard

Specifies the short standard name style; for example, “CST” for the Central time zone.

case daylightSaving

Specifies the daylight saving name style; for example, “Central Daylight Time” for the Central time zone.

case shortDaylightSaving

Specifies the short daylight saving name style; for example, “CDT” for the Central time zone.

case generic

Specifies the generic name style, which does not distinguish between daylight saving and standard time; for example, “Central Time” for the Central time zone.

case shortGeneric

Specifies the short generic name style, which does not distinguish between daylight saving and standard time; for example, “CT” for the Central time zone.

## See Also

### Constants

Notification Name

Name of the notification posted when the time zone changes.

