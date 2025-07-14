

- Foundation
- Date
- 
  - Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
- Date.FormatStyle.Symbol.SecondFraction
-  milliseconds(\_:) 

Type Method

# milliseconds(\_:)

Creates a custom format style representing the milliseconds elapsed in a day.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func milliseconds(_ val: Int) -> Date.FormatStyle.Symbol.SecondFraction
```

## Parameters 

`val`  

Length of the string representation of the number of milliseconds elapsed in a day.

## Return Value

Returns the number of milliseconds elapsed in the day.

## See Also

### Modifying a Second Fraction

static func fractional(Int) -> Date.FormatStyle.Symbol.SecondFraction

Creates a custom format style representing the fractional seconds component of a date.

