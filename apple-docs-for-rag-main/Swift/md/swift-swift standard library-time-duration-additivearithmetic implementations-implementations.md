

- Swift
- Swift Standard Library
- Time
- Duration
-  AdditiveArithmetic Implementations 

API Collection

# AdditiveArithmetic Implementations

## Topics

### Operators

static func + (Self) -> Self

Returns the given number unchanged.

static func + (Duration, Duration) -> Duration

Adds two values and produces their sum.

static func += (inout Duration, Duration)

Adds two values and stores the result in the left-hand-side variable.

static func += (inout Self, Self)

Adds two values and stores the result in the left-hand-side variable.

static func - (Duration, Duration) -> Duration

Subtracts one value from another and produces their difference.

static func -= (inout Duration, Duration)

Subtracts the second value from the first and stores the difference in the left-hand-side variable.

static func -= (inout Self, Self)

Subtracts the second value from the first and stores the difference in the left-hand-side variable.

### Type Properties

static var zero: Duration

The zero value.

