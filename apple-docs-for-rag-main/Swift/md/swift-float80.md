

- Swift
-  Float80 

Structure

# Float80

An extended-precision, floating-point value type.

macOS 10.10+

``` source
@frozen
struct Float80
```

## Overview

`Float80` is available on Intel when the target system supports an 80-bit long double type, and unavailable on Apple silicon.

## Topics

### Initializers

init()

init?(Substring)

init?(exactly: Double)

Creates a new instance initialized to the given value, if it can be represented without rounding.

init?(exactly: Float)

Creates a new instance initialized to the given value, if it can be represented without rounding.

init?(exactly: Float80)

Creates a new instance initialized to the given value, if it can be represented without rounding.

init(nan: Float80.RawSignificand, signaling: Bool)

Creates a NaN (“not a number”) value with the specified payload.

### Default Implementations

AdditiveArithmetic Implementations

BinaryFloatingPoint Implementations

Comparable Implementations

CustomDebugStringConvertible Implementations

CustomReflectable Implementations

CustomStringConvertible Implementations

Equatable Implementations

ExpressibleByFloatLiteral Implementations

ExpressibleByIntegerLiteral Implementations

FloatingPoint Implementations

Hashable Implementations

LosslessStringConvertible Implementations

Numeric Implementations

SignedNumeric Implementations

Strideable Implementations

TextOutputStreamable Implementations

## Relationships

### Conforms To

- AdditiveArithmetic
- BinaryFloatingPoint
- BitwiseCopyable
- CVarArg
- Comparable
- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Equatable
- ExpressibleByFloatLiteral
- ExpressibleByIntegerLiteral
- FloatingPoint
- Hashable
- LosslessStringConvertible
- Numeric
- Sendable
- SignedNumeric
- Strideable
- TextOutputStreamable

## See Also

### Floating-Point Values

struct Float16

A half-precision (16b), floating-point value type.

