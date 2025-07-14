

- Foundation
- Date
- 
  - Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
- Date.FormatStyle.Symbol.SecondFraction
-  fractional(\_:) 

Type Method

# fractional(\_:)

Creates a custom format style representing the fractional seconds component of a date.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func fractional(_ val: Int) -> Date.FormatStyle.Symbol.SecondFraction
```

## Parameters 

`val`  

Length of the string representation of the fractional seconds component.

## Return Value

Returns the numerical representation of the fractional component of the second.

## See Also

### Modifying a Second Fraction

static func milliseconds(Int) -> Date.FormatStyle.Symbol.SecondFraction

Creates a custom format style representing the milliseconds elapsed in a day.

