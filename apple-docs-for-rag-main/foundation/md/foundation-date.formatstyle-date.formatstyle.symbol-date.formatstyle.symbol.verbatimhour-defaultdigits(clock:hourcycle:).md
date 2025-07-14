

- Foundation
- Date
- 
  - Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
- Date.FormatStyle.Symbol.VerbatimHour
-  defaultDigits(clock:hourCycle:) 

Type Method

# defaultDigits(clock:hourCycle:)

Creates a custom format style portraying the minimum number of digits that represents the hour.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func defaultDigits(
    clock: Date.FormatStyle.Symbol.VerbatimHour.Clock,
    hourCycle: Date.FormatStyle.Symbol.VerbatimHour.HourCycle
) -> Date.FormatStyle.Symbol.VerbatimHour
```

## Parameters 

`clock`  

The clock representation.

`hourCycle`  

The start of the clock representation.

## Return Value

An hour format style customized according to the specified clock representation and the start of the clock representation.

## See Also

### Modifying a Verbatim Hour

static func twoDigits(clock: Date.FormatStyle.Symbol.VerbatimHour.Clock, hourCycle: Date.FormatStyle.Symbol.VerbatimHour.HourCycle) -> Date.FormatStyle.Symbol.VerbatimHour

Creates a custom format style portraying two digits that represent the hour.

