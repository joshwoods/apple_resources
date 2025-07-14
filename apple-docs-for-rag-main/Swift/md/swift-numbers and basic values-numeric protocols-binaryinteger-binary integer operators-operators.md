

- Swift
- Swift Standard Library
- 
  - Swift Standard Library
- Numbers and Basic Values
- Numeric Protocols
- BinaryInteger
-  Binary Integer Operators 

API Collection

# Binary Integer Operators

Perform arithmetic and bitwise operations or compare values.

## Topics

### Arithmetic

static func + (Self, Self) -> Self

Adds two values and produces their sum.

**Required**

static func - (Self, Self) -> Self

Subtracts one value from another and produces their difference.

**Required**

static func * (Self, Self) -> Self

Multiplies two values and produces their product.

**Required**

static func / (Self, Self) -> Self

Returns the quotient of dividing the first value by the second.

**Required**

### Arithmetic with Assignment

static func += (inout Self, Self)

Adds two values and stores the result in the left-hand-side variable.

**Required**

static func -= (inout Self, Self)

Subtracts the second value from the first and stores the difference in the left-hand-side variable.

**Required**

static func *= (inout Self, Self)

Multiplies two values and stores the result in the left-hand-side variable.

**Required**

static func /= (inout Self, Self)

Divides the first value by the second and stores the quotient in the left-hand-side variable.

**Required**

### Bitwise Operations

static func &amp; (Self, Self) -> Self

Returns the result of performing a bitwise AND operation on the two given values.

**Required** Default implementation provided.

static func &amp;= (inout Self, Self)

Stores the result of performing a bitwise AND operation on the two given values in the left-hand-side variable.

**Required**

static func ~ (Self) -> Self

Returns the inverse of the bits set in the argument.

**Required** Default implementation provided.

### Comparison

static func != &lt;Other>(Self, Other) -> Bool

Returns a Boolean value indicating whether the two given values are not equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

## See Also

### Performing Calculations

func quotientAndRemainder(dividingBy: Self) -> (quotient: Self, remainder: Self)

Returns the quotient and remainder of this value divided by the given value.

**Required** Default implementation provided.

func isMultiple(of: Self) -> Bool

Returns `true` if this value is a multiple of the given value, and `false` otherwise.

**Required** Default implementations provided.

