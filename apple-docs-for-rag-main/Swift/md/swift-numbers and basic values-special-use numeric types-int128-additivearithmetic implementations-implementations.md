

- Swift
- Swift Standard Library
- 
  - Swift Standard Library
- Numbers and Basic Values
- Special-Use Numeric Types
- Int128
-  AdditiveArithmetic Implementations 

API Collection

# AdditiveArithmetic Implementations

## Topics

### Operators

static func + (Self) -> Self

Returns the given number unchanged.

static func + (Int128, Int128) -> Int128

Adds two values and produces their sum.

static func += (inout Self, Self)

Adds two values and stores the result in the left-hand-side variable.

static func - (Int128, Int128) -> Int128

Subtracts one value from another and produces their difference.

static func -= (inout Self, Self)

Subtracts the second value from the first and stores the difference in the left-hand-side variable.

### Type Properties

static var zero: Int128

The zero value.

static var zero: Self

The zero value.

