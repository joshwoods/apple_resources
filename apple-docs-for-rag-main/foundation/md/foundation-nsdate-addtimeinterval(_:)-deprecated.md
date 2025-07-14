

- Foundation
- NSDate
-  addTimeInterval(\_:) Deprecated

Instance Method

# addTimeInterval(\_:)

Returns a new date object that is set to a given number of seconds relative to the receiver.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func addTimeInterval(_ seconds: TimeInterval) -> Any
```

Deprecated

Use addingTimeInterval(_:) instead.

## Parameters 

`seconds`  

The number of seconds to add to the receiver. Use a negative value for seconds to have the returned object specify a date before the receiver.

## Return Value

A new NSDate object that is set to `seconds` seconds relative to the receiver. The date returned might have a representation different from the receiver’s.

## See Also

### Related Documentation

convenience init(timeInterval: TimeInterval, sinceDate: Date)

Returns a date object initialized relative to another given date by a given number of seconds.

func addingTimeInterval(TimeInterval) -> Self

Returns a new date object that is set to a given number of seconds relative to the receiver.

func timeIntervalSince(Date) -> TimeInterval

Returns the interval between the receiver and another given date.

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

func date(withCalendarFormat: String?, timeZone: TimeZone?) -> NSCalendarDate

Converts the receiver to a calendar date with a given format string and time zone.

Deprecated

func description(withCalendarFormat: String?, timeZone: TimeZone?, locale: Any?) -> String?Deprecated

