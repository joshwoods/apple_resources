

- Foundation
- Date
- 
  - Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
- Date.FormatStyle.Symbol.Day
-  julianModified(minimumLength:) 

Type Method

# julianModified(minimumLength:)

Creates a custom day format style representing the modified Julian day.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func julianModified(minimumLength: Int = 1) -> Date.FormatStyle.Symbol.Day
```

## Parameters 

`minimumLength`  

Specifies the minimum number of digits.

## Return Value

The minimum length specifies the minimum number of digits, zero-padded if necessary. For example, `002451334`.

## See Also

### Modifying a Day Format

static var defaultDigits: Date.FormatStyle.Symbol.Day

Custom format style portraying the minimum number of digits that represents the numeric day of month.

static var ordinalOfDayInMonth: Date.FormatStyle.Symbol.Day

Custom format style portraying the ordinal of the day in the month.

static var twoDigits: Date.FormatStyle.Symbol.Day

Custom format style portraying the two-digit numeric day of month, zero-padded if necessary.

