

- Foundation
- FormatStyle
-  currency(code:) 

Type Method

# currency(code:)

Returns a format style to use decimal currency notation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func currency(code: String) -> Self
```

Available when `Self` is `Decimal.FormatStyle.Currency`.

## Parameters 

`code`  

The currency code to use, such as `EUR` or `JPY`. See ISO-4217 for a list of valid codes.

## Return Value

A decimal format style that uses the specified currency code.

## Discussion

Use the dot-notation form of this method when the call point allows the use of Decimal.FormatStyle. You typically do this when calling the formatted(_:) method of Decimal.

The following example creates an array of decimals, then uses formatted(_:) and the currency style provided by this method to format the values as US dollars.

```
let nums: [Decimal] = [100.01, 1000.02, 10000.03, 100000.04, 1000000.05]
let currencyNums = nums.map { $0.formatted(
    .currency(code:"USD")) } // ["$100.01", "$1,000.02", "$10,000.03", "$100,000.04", "$1,000,000.05"]
```

## See Also

### Applying currency styles

static func currency&lt;V>(code: String) -> Self

Returns a format style to use integer currency notation.

static func currency&lt;Value>(code: String) -> Self

Returns a format style to use floating-point currency notation.

