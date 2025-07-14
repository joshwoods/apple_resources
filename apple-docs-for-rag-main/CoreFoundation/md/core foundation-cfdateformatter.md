

- Core Foundation
-  CFDateFormatter 

Class

# CFDateFormatter

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFDateFormatter
```

## Overview

CFDateFormatter objects format the textual representations of CFDate and CFAbsoluteTime objects, and convert textual representations of dates and times into CFDate and CFAbsoluteTime objects. You can express the representation of dates and times very flexibly, for example “Thu 22 Dec 1994” is just as acceptable as “12/22/94.” You specify how strings are formatted and parsed by setting a format string and other properties of a CFDateFomatter object.

The format of the format string itself is defined by Unicode Technical Standard \#35; the version of the standard used varies with release of the operating system, and is described in Introduction to Data Formatting Programming Guide For Cocoa.

Note

CFDateFormatter is not thread safe, so you must not mutate a given date formatter simultaneously from multiple threads.

## Topics

### Creating a Date Formatter

func CFDateFormatterCreate(CFAllocator!, CFLocale!, CFDateFormatterStyle, CFDateFormatterStyle) -> CFDateFormatter!

Creates a new CFDateFormatter object, localized to the given locale, which will format dates to the given date and time styles.

### Configuring a Date Formatter

func CFDateFormatterSetFormat(CFDateFormatter!, CFString!)

Sets the format string of the given date formatter to the specified value.

func CFDateFormatterSetProperty(CFDateFormatter!, CFString!, CFTypeRef!)

Sets a date formatter property using a key-value pair.

### Parsing Strings

func CFDateFormatterCreateDateFromString(CFAllocator!, CFDateFormatter!, CFString!, UnsafeMutablePointer&lt;CFRange>!) -> CFDate!

Returns a date object representing a given string.

func CFDateFormatterGetAbsoluteTimeFromString(CFDateFormatter!, CFString!, UnsafeMutablePointer&lt;CFRange>!, UnsafeMutablePointer&lt;CFAbsoluteTime>!) -> Bool

Returns an absolute time object representing a given string.

### Creating Strings From Data

func CFDateFormatterCreateStringWithAbsoluteTime(CFAllocator!, CFDateFormatter!, CFAbsoluteTime) -> CFString!

Returns a string representation of the given absolute time using the specified date formatter.

func CFDateFormatterCreateStringWithDate(CFAllocator!, CFDateFormatter!, CFDate!) -> CFString!

Returns a string representation of the given date using the specified date formatter.

func CFDateFormatterCreateDateFormatFromTemplate(CFAllocator!, CFString!, CFOptionFlags, CFLocale!) -> CFString!

Returns a localized date format string representing the given date format components arranged appropriately for the specified locale.

### Getting Information About a Date Formatter

func CFDateFormatterCopyProperty(CFDateFormatter!, CFDateFormatterKey!) -> CFTypeRef!

Returns a copy of a date formatter’s value for a given key.

func CFDateFormatterGetDateStyle(CFDateFormatter!) -> CFDateFormatterStyle

Returns the date style used to create the given date formatter object.

func CFDateFormatterGetFormat(CFDateFormatter!) -> CFString!

Returns a format string for the given date formatter object.

func CFDateFormatterGetLocale(CFDateFormatter!) -> CFLocale!

Returns the locale object used to create the given date formatter object.

func CFDateFormatterGetTimeStyle(CFDateFormatter!) -> CFDateFormatterStyle

Returns the time style used to create the given date formatter object.

### Getting the CFDateFormatter Type ID

func CFDateFormatterGetTypeID() -> CFTypeID

Returns the type identifier for CFDateFormatter.

### Data Types

enum CFDateFormatterStyle

Data type for predefined date and time format styles.

### Constants

Date Formatter Styles

Predefined date and time format styles.

Date Formatter Property Keys

Keys used in key-value pairs to discover and specify the value of date formatter properties—used in conjunction with CFDateFormatterCopyProperty(_:_:) and CFDateFormatterSetProperty(_:_:_:).

Calendar Names

Calendar names used by CFDateFormatter.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Related Documentation

Data Formatting Guide for Core Foundation

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

class CFDictionary

class CFError

class CFFileDescriptor

