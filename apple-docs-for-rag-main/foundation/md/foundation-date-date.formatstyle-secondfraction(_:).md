

- Foundation
- Date
- Date.FormatStyle
-  secondFraction(\_:) 

Instance Method

# secondFraction(\_:)

Modifies the date format style to use the specified second fraction format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func secondFraction(_ format: Date.FormatStyle.Symbol.SecondFraction) -> Date.FormatStyle
```

## Parameters 

`format`  

The second fraction format style applied to the date format style.

## Return Value

A date format style modified to include the specified second fraction style.

## Discussion

Static methods that return Date.FormatStyle.Symbol.SecondFraction objects include fractional(_:) and milliseconds(_:).

This example shows a variety of Date.FormatStyle.Symbol.SecondFraction format styles applied to a date:

```
let meetingDate = Date() // Feb 9, 2021 at 3:05:41.827 PM
meetingDate.formatted(Date.FormatStyle().secondFraction(.fractional(3))) // 827
meetingDate.formatted(Date.FormatStyle().secondFraction(.fractional(1))) // 8
meetingDate.formatted(Date.FormatStyle().secondFraction(.milliseconds(4))) // 11122827
```

For more information about formatting dates, see Date.FormatStyle.

## See Also

### Specifying the Time Format

func hour(Date.FormatStyle.Symbol.Hour) -> Date.FormatStyle

Modifies the date format style to use the specified hour format style.

func minute(Date.FormatStyle.Symbol.Minute) -> Date.FormatStyle

Modifies the date format style to use the specified minute format style.

func second(Date.FormatStyle.Symbol.Second) -> Date.FormatStyle

Modifies the date format style to use the specified second format style.

func timeZone(Date.FormatStyle.Symbol.TimeZone) -> Date.FormatStyle

Modifies the date format style to use the specified time zone format style.

struct TimeStyle

Type that defines time styles varied in length or components included.

