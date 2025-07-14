

- Foundation
- Date
- 
  - Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
- Date.FormatStyle.Symbol.Hour
-  twoDigitsNoAMPM 

Type Property

# twoDigitsNoAMPM

Custom format style portraying the numeric hour using two digits.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var twoDigitsNoAMPM: Date.FormatStyle.Symbol.Hour { get }
```

## Discussion

This style pads the hour with a leading zero if necessary. It doesn’t include the day period symbol (a.m. or p.m.). For example, `01`, `11`.

## See Also

### Modifying an Hour

static var defaultDigitsNoAMPM: Date.FormatStyle.Symbol.Hour

Custom format style portraying the minimum number of digits that represents the numeric hour.

Deprecated

static func conversationalDefaultDigits(amPM: Date.FormatStyle.Symbol.Hour.AMPMStyle) -> Date.FormatStyle.Symbol.Hour

Custom format style portraying the minimum number of digits that represents the hour and locale-dependent conversational day period formats.

static func conversationalTwoDigits(amPM: Date.FormatStyle.Symbol.Hour.AMPMStyle) -> Date.FormatStyle.Symbol.Hour

Custom format style portraying two digits that represent the hour and locale-dependent conversational day period formats.

static func defaultDigits(amPM: Date.FormatStyle.Symbol.Hour.AMPMStyle) -> Date.FormatStyle.Symbol.Hour

Custom format style portraying the minimum number of digits that represents the hour and locale-dependent day period formats.

static func twoDigits(amPM: Date.FormatStyle.Symbol.Hour.AMPMStyle) -> Date.FormatStyle.Symbol.Hour

Custom format style portraying two digits that represent the hour and locale-dependent day period formats.

