

- Foundation
- Date
- Date.FormatStyle
-  timeZone(\_:) 

Instance Method

# timeZone(\_:)

Modifies the date format style to use the specified time zone format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func timeZone(_ format: Date.FormatStyle.Symbol.TimeZone = .specificName(.short)) -> Date.FormatStyle
```

## Parameters 

`format`  

The time zone format style applied to the date format style.

## Return Value

A date format style modified to include the specified time zone format style.

## Discussion

Values of Date.FormatStyle.Symbol.TimeZone are exemplarLocation and genericLocation.

Static methods that return Date.FormatStyle.Symbol.TimeZone objects include````  ```Date/FormatStyle/Symbol/TimeZone/genericName(_:)```, ```` ```` Date/FormatStyle/Symbol/TimeZone/identifier(_:)```,`  ````Date/FormatStyle/Symbol/TimeZone/iso8601(\_:)``` ,` ``Date/FormatStyle/Symbol/TimeZone/localizedGMT(_:) ```,````  and ``Date/FormatStyle/Symbol/TimeZone/specificName(_:)```. ````

## See Also

### Specifying the Time Format

func hour(Date.FormatStyle.Symbol.Hour) -> Date.FormatStyle

Modifies the date format style to use the specified hour format style.

func minute(Date.FormatStyle.Symbol.Minute) -> Date.FormatStyle

Modifies the date format style to use the specified minute format style.

func second(Date.FormatStyle.Symbol.Second) -> Date.FormatStyle

Modifies the date format style to use the specified second format style.

func secondFraction(Date.FormatStyle.Symbol.SecondFraction) -> Date.FormatStyle

Modifies the date format style to use the specified second fraction format style.

struct TimeStyle

Type that defines time styles varied in length or components included.

