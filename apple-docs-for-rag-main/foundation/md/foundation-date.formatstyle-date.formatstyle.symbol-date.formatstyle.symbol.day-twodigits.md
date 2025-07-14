

- Foundation
- Date
- 
  - Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
- Date.FormatStyle.Symbol.Day
-  twoDigits 

Type Property

# twoDigits

Custom format style portraying the two-digit numeric day of month, zero-padded if necessary.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var twoDigits: Date.FormatStyle.Symbol.Day { get }
```

## Discussion

This style produces `01` for the first day of the month and `18` for the eighteenth. To use single digits when possible, use defaultDigits.

## See Also

### Modifying a Day Format

static var defaultDigits: Date.FormatStyle.Symbol.Day

Custom format style portraying the minimum number of digits that represents the numeric day of month.

static var ordinalOfDayInMonth: Date.FormatStyle.Symbol.Day

Custom format style portraying the ordinal of the day in the month.

static func julianModified(minimumLength: Int) -> Date.FormatStyle.Symbol.Day

Creates a custom day format style representing the modified Julian day.

