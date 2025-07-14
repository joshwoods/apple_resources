

- Foundation
-  NSDecimalMaxSize 

Global Variable

# NSDecimalMaxSize

The maximum size of Decimal.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var NSDecimalMaxSize: Int32 { get }
```

## Discussion

Gives a precision of at least 38 decimal digits, 128 binary positions.

## See Also

### Getting particular decimals

static let greatestFiniteMagnitude: Decimal

The decimal that contains the largest possible non-infinite magnitude for the underlying representation.

static let leastFiniteMagnitude: Decimal

The decimal that contains the smallest possible non-infinite magnitude for the underlying representation.

static let leastNonzeroMagnitude: Decimal

The decimal value that represents the smallest possible non-zero value for the underlying representation.

static let leastNormalMagnitude: Decimal

The decimal value that represents the smallest possible normal magnitude for the underlying representation.

static let pi: Decimal

The mathematical constant pi.

static var nan: Decimal

The value that represents “not a number.”

static var quietNaN: Decimal

A quiet representation of not-a-number.

static var radix: Int

The radix used by decimal numbers.

var NSDecimalNoScale: Int32

Specifies that the number of digits allowed after the decimal separator in a decimal number should not be limited.

