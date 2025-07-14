

- Foundation
- NSDate
-  date(withNaturalLanguageString:locale:) Deprecated

Type Method

# date(withNaturalLanguageString:locale:)

Creates and returns a date object set to the date and time specified by a given string.

iOS 2.0–8.0DeprecatediPadOS 2.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.4–10.10Deprecated

``` source
class func date(
    withNaturalLanguageString string: String,
    locale: Any?
) -> Any?
```

Deprecated

Create an NSDateFormatter with \`init\` and set the dateFormat property instead.

## Parameters 

`string`  

A string that contains a colloquial specification of a date, such as “last Tuesday at dinner,” “3pm December 31, 2001,” “12/31/01,” or “31/12/01.”

`locale`  

An `NSDictionary` object containing locale data. To use the user’s preferences, you can use `[[NSUserDefaults standardUserDefaults] dictionaryRepresentation]`.

If you pass `nil` or an instance of `NSLocale`, `NSDate` uses the system default locale—this is not the same as the current user’s locale.

## Return Value

A new `NSDate` object set to the date and time specified by `string` as interpreted according to `locale`.

## Discussion

This method supports only a limited set of colloquial phrases, primarily in English. It may give unexpected results, and its use is strongly discouraged. To create a date object from a string, you should use a date formatter object instead (see DateFormatter and Data Formatting Guide).

The keys and values that represent the locale data from `locale` are used when parsing the string. In addition to the locale keys listed in the class description, these keys are used when parsing natural language strings:

- NSDateTimeOrdering

- NSEarlierTimeDesignations

- NSHourNameDesignations

- NSLaterTimeDesignations

- NSNextDayDesignations

- NSNextNextDayDesignations

- NSPriorDayDesignations

- NSThisDayDesignations

- NSYearMonthWeekDesignations

## See Also

### Legacy Operations

class func date(withNaturalLanguageString: String) -> Any?

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

func description(withCalendarFormat: String?, timeZone: TimeZone?, locale: Any?) -> String?Deprecated

