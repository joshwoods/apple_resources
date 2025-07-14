

- Foundation
- Date
- 
  - Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
- Date.FormatStyle.Symbol.Second
-  twoDigits 

Type Property

# twoDigits

The custom format style that conveys a two-digit numeric second, zero-padded if necessary.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var twoDigits: Date.FormatStyle.Symbol.Second { get }
```

## Discussion

This style represents the seconds field like `01` or `18`.

## See Also

### Modifying a Second

static var defaultDigits: Date.FormatStyle.Symbol.Second

The custom format style that conveys the minimum number of digits that represents the numeric second.

