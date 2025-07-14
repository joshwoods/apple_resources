

- Foundation
- NSDate
-  date(withCalendarFormat:timeZone:) Deprecated

Instance Method

# date(withCalendarFormat:timeZone:)

Converts the receiver to a calendar date with a given format string and time zone.

iOS 2.0–8.0DeprecatediPadOS 2.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.4–10.10Deprecated

``` source
func date(
    withCalendarFormat format: String?,
    timeZone aTimeZone: TimeZone?
) -> NSCalendarDate
```

Deprecated

Use NSDate methods to set the individual date values.

## Parameters 

`format`  

The format for the returned string (see Date and Number Formatters in OS X v10.0 to 10.3 for a discussion of how to create the format string). Pass `nil` to use the default format string, “`%Y-%m-%d %H:%M:%S %z`” (this conforms to the international format `YYYY-MM-DD HH:MM:SS ±HHMM`.)

`aTimeZone`  

The time zone for the new calendar date. Pass `nil` to use the default time zone—specific to the current locale.

## Return Value

A new NSCalendarDate object bound to `format` and the time zone `aTimeZone`.

## See Also

### Legacy Operations

class func date(withNaturalLanguageString: String) -> Any?

Creates and returns a date object set to the date and time specified by a given string.

Deprecated

class func date(withNaturalLanguageString: String, locale: Any?) -> Any?

Creates and returns a date object set to the date and time specified by a given string.

Deprecated

class func date(with: String) -> Any

Creates and returns a date object with a date and time value specified by a given string in the international string representation format (`YYYY-MM-DD HH:MM:SS ±HHMM`).

Deprecated

convenience init?(string: String)

Returns a date object initialized with a date and time value specified by a given string in the international string representation format.

Deprecated

func addTimeInterval(TimeInterval) -> Any

Returns a new date object that is set to a given number of seconds relative to the receiver.

Deprecated

func description(withCalendarFormat: String?, timeZone: TimeZone?, locale: Any?) -> String?Deprecated

