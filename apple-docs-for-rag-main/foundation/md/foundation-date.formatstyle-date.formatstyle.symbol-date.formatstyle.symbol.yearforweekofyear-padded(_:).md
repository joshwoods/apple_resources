

- Foundation
- Date
- 
  - Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
- Date.FormatStyle.Symbol.YearForWeekOfYear
-  padded(\_:) 

Type Method

# padded(\_:)

Returns a custom format style that represents the three or more digits of the year in week-of-year calendars, zero-padded if necessary.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func padded(_ length: Int) -> Date.FormatStyle.Symbol.YearForWeekOfYear
```

## Parameters 

`length`  

The length of the string to display a calendar year.

## Return Value

A custom year format style that portrays the year of a week of year calendar system with the provided length.

## See Also

### Modifying a Year for Week-of-Year

static var defaultDigits: Date.FormatStyle.Symbol.YearForWeekOfYear

Custom week of the year format style showing the minimum number of digits that represents the year in week-of-year calendars.

static var twoDigits: Date.FormatStyle.Symbol.YearForWeekOfYear

The custom format style that represents the two-digit numeric year in week-of-year calendars, zero-padded or truncated if necessary.

