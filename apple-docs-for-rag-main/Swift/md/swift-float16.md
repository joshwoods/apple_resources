

- Swift
-  Float16 

Structure

# Float16

A half-precision (16b), floating-point value type.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@frozen
struct Float16
```

## Overview

`Float16` is available on Apple silicon, and unavailable on Intel when targeting macOS.

## Topics

### Initializers

init()

init?(Substring)

init(Float16)

Creates a new instance initialized to the given value.

init(bitPattern: UInt16)

Creates a new value with the given bit pattern.

init?(exactly: Float16)

Creates a new instance initialized to the given value, if it can be represented without rounding.

init?(exactly: Double)

Creates a new instance initialized to the given value, if it can be represented without rounding.

init?(exactly: Float)

Creates a new instance initialized to the given value, if it can be represented without rounding.

init(nan: Float16.RawSignificand, signaling: Bool)

Creates a NaN (“not a number”) value with the specified payload.

### Instance Properties

var bitPattern: UInt16

The bit pattern of the value’s encoding.

### Default Implementations

AdditiveArithmetic Implementations

AtomicRepresentable Implementations

BinaryFloatingPoint Implementations

Comparable Implementations

CustomDebugStringConvertible Implementations

CustomStringConvertible Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

ExpressibleByFloatLiteral Implementations

ExpressibleByIntegerLiteral Implementations

FloatingPoint Implementations

Hashable Implementations

LosslessStringConvertible Implementations

Numeric Implementations

SIMDScalar Implementations

SignedNumeric Implementations

Strideable Implementations

TextOutputStreamable Implementations

## Relationships

### Conforms To

- AdditiveArithmetic
- AtomicRepresentable
- BNNSScalar
- BinaryFloatingPoint
- BitwiseCopyable
- Comparable
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- ExpressibleByFloatLiteral
- ExpressibleByIntegerLiteral
- FloatingPoint
- Hashable
- LosslessStringConvertible
- MLShapedArrayScalar
- MLTensorScalar
- Numeric
- Plottable
- PrimitivePlottableProtocol
- SIMDScalar
- Sendable
- SignedNumeric
- Strideable
- TextOutputStreamable

## See Also

### Floating-Point Values

struct Float80

An extended-precision, floating-point value type.

