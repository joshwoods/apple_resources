

- Foundation
- Date
- 
  - Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
- Date.FormatStyle.Symbol.Year
-  relatedGregorian(minimumLength:) 

Type Method

# relatedGregorian(minimumLength:)

Returns a custom format style that portrays the year of a non-Gregorian calendar system in the corresponding Gregorian year.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func relatedGregorian(minimumLength: Int = 1) -> Date.FormatStyle.Symbol.Year
```

## Parameters 

`minimumLength`  

The minimum length to display the full year.

## Return Value

A custom year format style that portrays the year of the calendar system with the provided minimum length.

## Discussion

For non-Gregorian calendars, output corresponds to the extended Gregorian year in which the calendar’s year begins. The default length is the minimum needed to show the full year.

## See Also

### Modifying a Year

static var defaultDigits: Date.FormatStyle.Symbol.Year

The custom year format style showing the minimum number of digits that represents the numeric year.

static var twoDigits: Date.FormatStyle.Symbol.Year

The custom format style portraying the two-digit numeric year, zero-padded if necessary.

static func padded(Int) -> Date.FormatStyle.Symbol.Year

Returns a custom format style that portrays the year of the calendar system of the provided length, zero-padded if necessary.

static func extended(minimumLength: Int) -> Date.FormatStyle.Symbol.Year

Returns a custom format style that portrays the year of the calendar system, encompassing all supra-year fields.

