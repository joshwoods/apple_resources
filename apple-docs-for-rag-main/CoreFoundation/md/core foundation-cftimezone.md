

- Core Foundation
-  CFTimeZone 

Class

# CFTimeZone

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFTimeZone
```

## Overview

CFTimeZone defines the behavior of time zone objects. Time zone objects represent geopolitical regions. Consequently, these objects have names for these regions. Time zone objects also represent a temporal offset, either plus or minus, from Greenwich Mean Time (GMT) and an abbreviation (such as PST for Pacific Standard Time).

CFTimeZone provides several functions to create time zone objects: CFTimeZoneCreateWithName(_:_:_:) and CFTimeZoneCreateWithTimeIntervalFromGMT(_:_:). CFTimeZone also permits you to set the default time zone within your application using the CFTimeZoneSetDefault(_:) function. You can access this default time zone at any time with the CFTimeZoneCopyDefault() function.

CFTimeZone is “toll-free bridged” with its Cocoa Foundation counterpart, NSTimeZone. This means that the Core Foundation type is interchangeable in function or method calls with the bridged Foundation object. Therefore, in a method where you see an `NSTimeZone *` parameter, you can pass in a `CFTimeZoneRef`, and in a function where you see a `CFTimeZoneRef` parameter, you can pass in an NSTimeZone instance. This fact also applies to concrete subclasses of NSTimeZone. See Toll-Free Bridged Types for more information on toll-free bridging.

## Topics

### Creating a Time Zone

func CFTimeZoneCreateWithName(CFAllocator!, CFString!, Bool) -> CFTimeZone!

Returns the time zone object identified by a given name or abbreviation.

func CFTimeZoneCreateWithTimeIntervalFromGMT(CFAllocator!, CFTimeInterval) -> CFTimeZone!

Returns a time zone object for the specified time interval offset from Greenwich Mean Time (GMT).

func CFTimeZoneCreate(CFAllocator!, CFString!, CFData!) -> CFTimeZone!

Creates a time zone with a given name and data.

### System and Default Time Zones and Information

func CFTimeZoneCopyAbbreviationDictionary() -> CFDictionary!

Returns a dictionary holding the mappings of time zone abbreviations to time zone names.

func CFTimeZoneCopyAbbreviation(CFTimeZone!, CFAbsoluteTime) -> CFString!

Returns the abbreviation of a time zone at a specified date.

func CFTimeZoneCopyDefault() -> CFTimeZone!

Returns the default time zone set for your application.

func CFTimeZoneCopySystem() -> CFTimeZone!

Returns the time zone currently used by the system.

func CFTimeZoneSetDefault(CFTimeZone!)

Sets the default time zone for your application the given time zone.

func CFTimeZoneCopyKnownNames() -> CFArray!

Returns an array of strings containing the names of all the time zones known to the system.

func CFTimeZoneResetSystem()

Clears the previously determined system time zone, if any.

func CFTimeZoneSetAbbreviationDictionary(CFDictionary!)

Sets the abbreviation dictionary to a given dictionary.

### Getting Information About Time Zones

func CFTimeZoneGetName(CFTimeZone!) -> CFString!

Returns the geopolitical region name that identifies a given time zone.

func CFTimeZoneCopyLocalizedName(CFTimeZone!, CFTimeZoneNameStyle, CFLocale!) -> CFString!

Returns the localized name of a given time zone.

func CFTimeZoneGetSecondsFromGMT(CFTimeZone!, CFAbsoluteTime) -> CFTimeInterval

Returns the difference in seconds between the receiver and Greenwich Mean Time (GMT) at the specified date.

func CFTimeZoneGetData(CFTimeZone!) -> CFData!

Returns the data that stores the information used by a time zone.

### Getting Daylight Savings Time Information

func CFTimeZoneIsDaylightSavingTime(CFTimeZone!, CFAbsoluteTime) -> Bool

Returns whether or not a time zone is in daylight savings time at a specified date.

func CFTimeZoneGetDaylightSavingTimeOffset(CFTimeZone!, CFAbsoluteTime) -> CFTimeInterval

Returns the daylight saving time offset for a time zone at a given time.

func CFTimeZoneGetNextDaylightSavingTimeTransition(CFTimeZone!, CFAbsoluteTime) -> CFAbsoluteTime

Returns the time in a given time zone of the next daylight saving time transition after a given time.

### Getting the CFTimeZone Type ID

func CFTimeZoneGetTypeID() -> CFTypeID

Returns the type identifier for the CFTimeZone opaque type.

### Data Types

enum CFTimeZoneNameStyle

Index type for constants used to specify styles of time zone names.

### Constants

Notification Name

Name of the notification posted when the time zone changes.

Time Zone Name Styles

Constants to specify styles for time zone names.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Related Documentation

Date and Time Programming Guide for Core Foundation

### Opaque Types

class CFAllocator

class CFArray

class CFAttributedString

class CFBag

class CFBinaryHeap

class CFBitVector

class CFBoolean

class CFBundle

class CFCalendar

class CFCharacterSet

class CFData

class CFDate

class CFDateFormatter

class CFDictionary

class CFError

