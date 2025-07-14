

- Foundation
- Date
- 
  - Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
- Date.FormatStyle.Symbol.Hour
-  conversationalTwoDigits(amPM:) 

Type Method

# conversationalTwoDigits(amPM:)

Custom format style portraying two digits that represent the hour and locale-dependent conversational day period formats.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func conversationalTwoDigits(amPM: Date.FormatStyle.Symbol.Hour.AMPMStyle) -> Date.FormatStyle.Symbol.Hour
```

## Parameters 

`amPM`  

Specifies the format of the day period representation.

## Return Value

An hour format style customized according to the specified day period format style and the given locale.

## Discussion

This style pads the hour with a leading zero if necessary. This style may include the day period symbol (a.m. or p.m.), depending on locale, and can include conversational period formats. For example, `07a` (`narrow`), `07AM` (`abbreviated`), `07A.M.` (`wide`).

## See Also

### Modifying an Hour

static var defaultDigitsNoAMPM: Date.FormatStyle.Symbol.Hour

Custom format style portraying the minimum number of digits that represents the numeric hour.

Deprecated

static var twoDigitsNoAMPM: Date.FormatStyle.Symbol.Hour

Custom format style portraying the numeric hour using two digits.

Deprecated

static func conversationalDefaultDigits(amPM: Date.FormatStyle.Symbol.Hour.AMPMStyle) -> Date.FormatStyle.Symbol.Hour

Custom format style portraying the minimum number of digits that represents the hour and locale-dependent conversational day period formats.

static func defaultDigits(amPM: Date.FormatStyle.Symbol.Hour.AMPMStyle) -> Date.FormatStyle.Symbol.Hour

Custom format style portraying the minimum number of digits that represents the hour and locale-dependent day period formats.

static func twoDigits(amPM: Date.FormatStyle.Symbol.Hour.AMPMStyle) -> Date.FormatStyle.Symbol.Hour

Custom format style portraying two digits that represent the hour and locale-dependent day period formats.

