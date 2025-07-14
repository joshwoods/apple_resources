

- Foundation
- NumberFormatStyleConfiguration
- NumberFormatStyleConfiguration.Precision
-  significantDigits(\_:) 

Type Method

# significantDigits(\_:)

Returns a precision that constrains formatted values to a given number of significant digits.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func significantDigits(_ digits: Int) -> NumberFormatStyleConfiguration.Precision
```

## Parameters 

`digits`  

The maximum number of significant digits to use when formatting values.

## Return Value

A precision that constrains formatted values to a given number of significant digits.

## Discussion

When using this precision, the formatter rounds values that have more sigificant digits than the maximum of the range, as seen in the following example:

```
let myNum = 123456.formatted(.number
    .precision(.significantDigits(4))
    .rounded(rule: .down)) // "123,400"
```

## See Also

### Precision configurations

static func significantDigits&lt;R>(R) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values to a range of significant digits.

static func integerAndFractionLength&lt;R1, R2>(integerLimits: R1, fractionLimits: R2) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values to ranges of allowed digits in the integer and fraction parts.

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

