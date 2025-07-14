

- Foundation
- Date
- 
  - Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
- Date.FormatStyle.Symbol.Year
-  defaultDigits 

Type Property

# defaultDigits

The custom year format style showing the minimum number of digits that represents the numeric year.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var defaultDigits: Date.FormatStyle.Symbol.Year { get }
```

## Discussion

This style represents years like `1`, `18`, `202`, and `2020`.

## See Also

### Modifying a Year

static var twoDigits: Date.FormatStyle.Symbol.Year

The custom format style portraying the two-digit numeric year, zero-padded if necessary.

static func padded(Int) -> Date.FormatStyle.Symbol.Year

Returns a custom format style that portrays the year of the calendar system of the provided length, zero-padded if necessary.

static func relatedGregorian(minimumLength: Int) -> Date.FormatStyle.Symbol.Year

Returns a custom format style that portrays the year of a non-Gregorian calendar system in the corresponding Gregorian year.

static func extended(minimumLength: Int) -> Date.FormatStyle.Symbol.Year

Returns a custom format style that portrays the year of the calendar system, encompassing all supra-year fields.

