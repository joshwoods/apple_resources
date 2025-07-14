

- Foundation
- NumberFormatStyleConfiguration
- NumberFormatStyleConfiguration.Precision
-  integerAndFractionLength(integerLimits:fractionLimits:) 

Type Method

# integerAndFractionLength(integerLimits:fractionLimits:)

Returns a precision that constrains formatted values to ranges of allowed digits in the integer and fraction parts.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func integerAndFractionLength(
    integerLimits: R1,
    fractionLimits: R2
) -> NumberFormatStyleConfiguration.Precision where R1 : RangeExpression, R2 : RangeExpression, R1.Bound == Int, R2.Bound == Int
```

## Parameters 

`integerLimits`  

A range from the minimum to the maximum number of digits to use when formatting the integer part of a number.

`fractionLimits`  

A range from the minimum to the maximum number of digits to use when formatting the fraction part of a number.

## Return Value

A precision that constrains formatted values to ranges of digits in the integer and fraction parts.

## Discussion

When using this precision, the formatter rounds values that have more digits than the maximum of the range, as seen in the following example:

```
let myNum = 12345.6789.formatted(.number
    .precision(.integerAndFractionLength(integerLimits: 2...,
                                         fractionLimits: 2...3))
    .rounded(rule: .down)) // "12,345.678"
```

## See Also

### Precision configurations

static func significantDigits&lt;R>(R) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values to a range of significant digits.

static func significantDigits(Int) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values to a given number of significant digits.

static func integerAndFractionLength(integer: Int, fraction: Int) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values a given number of allowed digits in the integer and fraction parts.

static func integerLength&lt;R>(R) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values to a range of allowed digits in the integer part.

static func integerLength(Int) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values to a given number of allowed digits in the integer part.

static func fractionLength&lt;R>(R) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values to a range of allowed digits in the fraction part.

static func fractionLength(Int) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values to a given number of allowed digits in the fraction part.

