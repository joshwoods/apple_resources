

- Foundation
- NumberFormatStyleConfiguration
- NumberFormatStyleConfiguration.Precision
-  integerAndFractionLength(integer:fraction:) 

Type Method

# integerAndFractionLength(integer:fraction:)

Returns a precision that constrains formatted values a given number of allowed digits in the integer and fraction parts.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func integerAndFractionLength(
    integer: Int,
    fraction: Int
) -> NumberFormatStyleConfiguration.Precision
```

## Parameters 

`integer`  

The number of digits to use when formatting the integer part of a number.

`fraction`  

The number of digits to use when formatting the fraction part of a number.

## Return Value

A precision that constrains formatted values a given number of digits in the integer and fraction parts.

## Discussion

When using this precision, the formatter pads values with fewer digits than the specified digits for the integer or fraction parts. Similarly, it rounds values that have more digits than specified. The following example shows this behavior, padding the integer part while rounding the fraction:

```
let myNum = 12345.6789.formatted(.number
    .precision(.integerAndFractionLength(integer: 6,
                                         fraction: 3))
    .rounded(rule: .down)) // "012,345.678"
```

## See Also

### Precision configurations

static func significantDigits&lt;R>(R) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values to a range of significant digits.

static func significantDigits(Int) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values to a given number of significant digits.

static func integerAndFractionLength&lt;R1, R2>(integerLimits: R1, fractionLimits: R2) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values to ranges of allowed digits in the integer and fraction parts.

static func integerLength&lt;R>(R) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values to a range of allowed digits in the integer part.

static func integerLength(Int) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values to a given number of allowed digits in the integer part.

static func fractionLength&lt;R>(R) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values to a range of allowed digits in the fraction part.

static func fractionLength(Int) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values to a given number of allowed digits in the fraction part.

