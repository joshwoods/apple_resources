

- Swift
-  StaticBigInt 

Structure

# StaticBigInt

An immutable arbitrary-precision signed integer.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
@frozen
struct StaticBigInt
```

## Overview

`StaticBigInt` is primarily intended to be used as the associated type of an `ExpressibleByIntegerLiteral` conformance.

```
extension UInt256: ExpressibleByIntegerLiteral {
    public init(integerLiteral value: StaticBigInt) {
        precondition(
            value.signum() >= 0 && value.bitWidth 

## Topics

### Instance Properties

var bitWidth: Int

Returns the minimal number of bits in this value’s binary representation, including the sign bit, and excluding the sign extension.

### Instance Methods

func signum() -> Int

Indicates the value’s sign.

### Subscripts

subscript(Int) -> UInt

Returns a 32-bit or 64-bit word of this value’s binary representation.

### Type Aliases

typealias IntegerLiteralType

A type that represents an integer literal.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomReflectable Implementations

ExpressibleByIntegerLiteral Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- ExpressibleByIntegerLiteral
- Sendable

## See Also

### Value Literals

protocol ExpressibleByIntegerLiteral

A type that can be initialized with an integer literal.

protocol ExpressibleByFloatLiteral

A type that can be initialized with a floating-point literal.

protocol ExpressibleByBooleanLiteral

A type that can be initialized with the Boolean literals `true` and `false`.

protocol ExpressibleByNilLiteral

A type that can be initialized using the nil literal, `nil`.

