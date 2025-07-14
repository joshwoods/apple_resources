

- Foundation
- FormatStyle
-  number 

Type Property

# number

A style for formatting decimal values.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var number: Decimal.FormatStyle { get }
```

Available when `Self` is `Decimal.FormatStyle`.

## Discussion

Use this type property when the call point allows the use of Decimal.FormatStyle. You typically do this when calling the formatted(_:) method of Decimal.

## See Also

### Applying numeric styles for decimals

struct FormatStyle

A structure that converts between decimal values and their textual representations.

