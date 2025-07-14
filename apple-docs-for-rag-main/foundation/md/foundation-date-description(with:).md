

- Foundation
- Date
-  description(with:) 

Instance Method

# description(with:)

Returns a string representation of the receiver using the given locale.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func description(with locale: Locale?) -> String
```

## Parameters 

`locale`  

A `Locale`. If you pass `nil`, `Date` formats the date in the same way as the `description` property.

## Return Value

A string representation of the `Date`, using the given locale, or if the locale argument is `nil`, in the international format `YYYY-MM-DD HH:MM:SS ±HHMM`, where `±HHMM` represents the time zone offset in hours and minutes from UTC (for example, “`2001-03-24 10:45:32 +0600`”).

## See Also

### Describing Dates

var description: String

The representation is useful for debugging only. There are a number of options to acquire a formatted string for a date including: date formatters (see NSDateFormatter and Data Formatting Guide), and the `Date` function `description(locale:)`.

var customPlaygroundQuickLook: PlaygroundQuickLook

A custom playground Quick Look for the date.

Deprecated

