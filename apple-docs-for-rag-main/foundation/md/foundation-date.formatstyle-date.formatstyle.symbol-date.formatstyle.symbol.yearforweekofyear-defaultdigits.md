

- Foundation
- Date
- 
  - Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
- Date.FormatStyle.Symbol.YearForWeekOfYear
-  defaultDigits 

Type Property

# defaultDigits

Custom week of the year format style showing the minimum number of digits that represents the year in week-of-year calendars.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var defaultDigits: Date.FormatStyle.Symbol.YearForWeekOfYear { get }
```

## Discussion

This represents week-of-year values like `1` or `18`.

## See Also

### Modifying a Year for Week-of-Year

static var twoDigits: Date.FormatStyle.Symbol.YearForWeekOfYear

The custom format style that represents the two-digit numeric year in week-of-year calendars, zero-padded or truncated if necessary.

static func padded(Int) -> Date.FormatStyle.Symbol.YearForWeekOfYear

Returns a custom format style that represents the three or more digits of the year in week-of-year calendars, zero-padded if necessary.

