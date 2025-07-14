

- Foundation
- NSDate
-  date(with:) Deprecated

Type Method

# date(with:)

Creates and returns a date object with a date and time value specified by a given string in the international string representation format (`YYYY-MM-DD HH:MM:SS ±HHMM`).

iOS 2.0–8.0DeprecatediPadOS 2.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.4–10.10Deprecated

``` source
class func date(with aString: String) -> Any
```

Deprecated

Use NSDateFormatter instead

## Parameters 

`aString`  

A string that specifies a date and time value in the international string representation format—`YYYY-MM-DD HH:MM:SS ±HHMM`, where `±HHMM` is a time zone offset in hours and minutes from UTC (for example, “`2001-03-24 10:45:32 +0600`”).

You must specify all fields of the format string, including the time zone offset, which must have a plus or minus sign prefix.

## Return Value

An `NSDate` object with a date and time value specified by `aString`.

## Discussion

To create a date object from a string, you should typically use a date formatter object instead (see DateFormatter and Data Formatting Guide).

## See Also

### Legacy Operations

class func date(withNaturalLanguageString: String) -> Any?

Creates and returns a date object set to the date and time specified by a given string.

Deprecated

class func date(withNaturalLanguageString: String, locale: Any?) -> Any?

Creates and returns a date object set to the date and time specified by a given string.

Deprecated

convenience init?(string: String)

Returns a date object initialized with a date and time value specified by a given string in the international string representation format.

Deprecated

func addTimeInterval(TimeInterval) -> Any

Returns a new date object that is set to a given number of seconds relative to the receiver.

Deprecated

func date(withCalendarFormat: String?, timeZone: TimeZone?) -> NSCalendarDate

Converts the receiver to a calendar date with a given format string and time zone.

Deprecated

func description(withCalendarFormat: String?, timeZone: TimeZone?, locale: Any?) -> String?Deprecated

