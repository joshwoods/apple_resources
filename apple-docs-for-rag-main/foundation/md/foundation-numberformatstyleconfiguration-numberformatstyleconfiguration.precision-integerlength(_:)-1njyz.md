

- Foundation
- NumberFormatStyleConfiguration
- NumberFormatStyleConfiguration.Precision
-  integerLength(\_:) 

Type Method

# integerLength(\_:)

Returns a precision that constrains formatted values to a given number of allowed digits in the integer part.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func integerLength(_ length: Int) -> NumberFormatStyleConfiguration.Precision
```

## Parameters 

`length`  

The number of digits to use when formatting the integer part of a number.

## Return Value

A precision that constrains formatted values to a given number of allowed digits in the integer part.

## See Also

### Precision configurations

static func significantDigits&lt;R>(R) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values to a range of significant digits.

static func significantDigits(Int) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values to a given number of significant digits.

static func integerAndFractionLength&lt;R1, R2>(integerLimits: R1, fractionLimits: R2) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values to ranges of allowed digits in the integer and fraction parts.

static func integerAndFractionLength(integer: Int, fraction: Int) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values a given number of allowed digits in the integer and fraction parts.

static func integerLength&lt;R>(R) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values to a range of allowed digits in the integer part.

static func fractionLength&lt;R>(R) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values to a range of allowed digits in the fraction part.

static func fractionLength(Int) -> NumberFormatStyleConfiguration.Precision

Returns a precision that constrains formatted values to a given number of allowed digits in the fraction part.

