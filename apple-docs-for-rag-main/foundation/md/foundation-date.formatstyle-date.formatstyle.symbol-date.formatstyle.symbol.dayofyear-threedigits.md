

- Foundation
- Date
- 
  - Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
- Date.FormatStyle.Symbol.DayOfYear
-  threeDigits 

Type Property

# threeDigits

Custom format style portraying the three-digit numeric day of the year, zero-padded if necessary.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var threeDigits: Date.FormatStyle.Symbol.DayOfYear { get }
```

## Discussion

For example, `001`, `018`, `317`.

## See Also

### Modifying a Day of Year Value

static var defaultDigits: Date.FormatStyle.Symbol.DayOfYear

Custom format style portraying the minimum number of digits that represents the numeric day of the year.

static var twoDigits: Date.FormatStyle.Symbol.DayOfYear

Custom format style portraying the two-digit numeric day of the year, zero-padded if necessary.

