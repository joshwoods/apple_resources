

- Foundation
- Date
- Date.FormatStyle
-  second(\_:) 

Instance Method

# second(\_:)

Modifies the date format style to use the specified second format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func second(_ format: Date.FormatStyle.Symbol.Second = .defaultDigits) -> Date.FormatStyle
```

## Parameters 

`format`  

The second format style applied to the date format style.

## Return Value

A date format style modified to include the specified second style.

## Discussion

Values of Date.FormatStyle.Symbol.Second are defaultDigits and twoDigits.

This example shows a variety of Date.FormatStyle.Symbol.Second format styles applied to a date:

```
let meetingDate = Date() // Feb 9, 2021 at 3:05 PM
meetingDate.formatted(Date.FormatStyle().second(.defaultDigits)) // 5
meetingDate.formatted(Date.FormatStyle().second(.twoDigits)) // 05
meetingDate.formatted(Date.FormatStyle().second()) // 5
```

If you don’t provide a format, the defaultDigits static variable is the default format.

For more information about formatting dates, see Date.FormatStyle.

## See Also

### Specifying the Time Format

func hour(Date.FormatStyle.Symbol.Hour) -> Date.FormatStyle

Modifies the date format style to use the specified hour format style.

func minute(Date.FormatStyle.Symbol.Minute) -> Date.FormatStyle

Modifies the date format style to use the specified minute format style.

func secondFraction(Date.FormatStyle.Symbol.SecondFraction) -> Date.FormatStyle

Modifies the date format style to use the specified second fraction format style.

func timeZone(Date.FormatStyle.Symbol.TimeZone) -> Date.FormatStyle

Modifies the date format style to use the specified time zone format style.

struct TimeStyle

Type that defines time styles varied in length or components included.

