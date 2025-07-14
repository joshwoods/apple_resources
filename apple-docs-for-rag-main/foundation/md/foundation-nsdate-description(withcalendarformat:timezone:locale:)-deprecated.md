

- Foundation
- NSDate
-  description(withCalendarFormat:timeZone:locale:) Deprecated

Instance Method

# description(withCalendarFormat:timeZone:locale:)

iOS 2.0–8.0DeprecatediPadOS 2.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.4–10.10Deprecated

``` source
func description(
    withCalendarFormat format: String?,
    timeZone aTimeZone: TimeZone?,
    locale: Any?
) -> String?
```

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

func date(withCalendarFormat: String?, timeZone: TimeZone?) -> NSCalendarDate

Converts the receiver to a calendar date with a given format string and time zone.

Deprecated

