

- Foundation
- Date
- Date.FormatStyle
-  hour(\_:) 

Instance Method

# hour(\_:)

Modifies the date format style to use the specified hour format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func hour(_ format: Date.FormatStyle.Symbol.Hour = .defaultDigits(amPM: .abbreviated)) -> Date.FormatStyle
```

## Parameters 

`format`  

The hour format style applied to the date format style.

## Return Value

A date format style modified to include the specified hour style.

## Discussion

Values of Date.FormatStyle.Symbol.Hour are defaultDigitsNoAMPM and twoDigitsNoAMPM.

Static methods that return Date.FormatStyle.Symbol.Hour objects include conversationalDefaultDigits(amPM:), conversationalTwoDigits(amPM:), defaultDigits(amPM:), and twoDigitsNoAMPM.

This example shows a variety of Date.FormatStyle.Symbol.Hour format styles applied to a date:

```
let meetingDate = Date() // Feb 9, 2021 at 7:00 PM
meetingDate.formatted(Date.FormatStyle().hour(.defaultDigitsNoAMPM)) 
// 7

meetingDate.formatted(Date.FormatStyle().hour(.twoDigitsNoAMPM)) 
// 07

meetingDate.formatted(Date.FormatStyle().hour(.defaultDigits(amPM: .narrow))) 
// 7p

meetingDate.formatted(Date.FormatStyle().hour(.twoDigits(amPM: .abbreviated))
// 07 PM

meetingDate.formatted(Date.FormatStyle().hour(.conversationalDefaultDigits(amPM: .wide))
// 7 P.M.
```

If you don’t provide a format, the defaultDigits static variable is the default format.

For more information about formatting dates, see Date.FormatStyle.

## See Also

### Specifying the Time Format

func minute(Date.FormatStyle.Symbol.Minute) -> Date.FormatStyle

Modifies the date format style to use the specified minute format style.

func second(Date.FormatStyle.Symbol.Second) -> Date.FormatStyle

Modifies the date format style to use the specified second format style.

func secondFraction(Date.FormatStyle.Symbol.SecondFraction) -> Date.FormatStyle

Modifies the date format style to use the specified second fraction format style.

func timeZone(Date.FormatStyle.Symbol.TimeZone) -> Date.FormatStyle

Modifies the date format style to use the specified time zone format style.

struct TimeStyle

Type that defines time styles varied in length or components included.

