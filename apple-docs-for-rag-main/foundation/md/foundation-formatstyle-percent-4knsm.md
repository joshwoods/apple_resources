

- Foundation
- FormatStyle
-  percent 

Type Property

# percent

A style for formatting decimal values as a percent represntation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var percent: Decimal.FormatStyle.Percent { get }
```

Available when `Self` is `Decimal.FormatStyle.Percent`.

## Discussion

Use this type property when the call point allows the use of Decimal.FormatStyle. You typically do this when calling the formatted(_:) method of Decimal.

## See Also

### Applying percentage styles for decimals

struct Percent

A format style that converts between decimal percentage values and their textual representations.

