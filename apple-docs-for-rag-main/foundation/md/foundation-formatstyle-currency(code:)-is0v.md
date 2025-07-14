

- Foundation
- FormatStyle
-  currency(code:) 

Type Method

# currency(code:)

Returns a format style to use integer currency notation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func currency(code: String) -> Self where Self == IntegerFormatStyle.Currency, V : BinaryInteger
```

## Parameters 

`code`  

The currency code to use, such as `EUR` or `JPY`. See ISO-4217 for a list of valid codes.

## Return Value

An integer format style that uses the specified currency code.

## Discussion

Use the dot-notation form of this method when the call point allows the use of IntegerFormatStyle. You typically do this when calling the `formatted` methods of types that conform to BinaryInteger.

The following example creates an array of integers, then uses formatted(_:) and the currency style provided by this method to format the integers as US dollars:

```
let nums: [Int] = [100, 1000, 10000, 100000, 1000000]
let currencyNums = nums.map { $0.formatted(
    .currency(code:"USD")) } // ["$100.00", "$1,000.00", "$10,000.00", "$100,000.00", "$1,000,000.00"]
```

## See Also

### Applying currency styles

static func currency&lt;Value>(code: String) -> Self

Returns a format style to use floating-point currency notation.

static func currency(code: String) -> Self

Returns a format style to use decimal currency notation.

