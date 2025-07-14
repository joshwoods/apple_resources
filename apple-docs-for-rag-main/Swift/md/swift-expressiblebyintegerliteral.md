

- Swift
-  ExpressibleByIntegerLiteral 

Protocol

# ExpressibleByIntegerLiteral

A type that can be initialized with an integer literal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol ExpressibleByIntegerLiteral
```

## Overview

The standard library integer and floating-point types, such as `Int` and `Double`, conform to the `ExpressibleByIntegerLiteral` protocol. You can initialize a variable or constant of any of these types by assigning an integer literal.

```
// Type inferred as 'Int'
let cookieCount = 12

// An array of 'Int'
let chipsPerCookie = [21, 22, 25, 23, 24, 19]

// A floating-point value initialized using an integer literal
let redPercentage: Double = 1
// redPercentage == 1.0
```

# Conforming to ExpressibleByIntegerLiteral

To add `ExpressibleByIntegerLiteral` conformance to your custom type, implement the required initializer.

## Topics

### Associated Types

associatedtype IntegerLiteralType : _ExpressibleByBuiltinIntegerLiteral

A type that represents an integer literal.

**Required**

### Initializers

init(integerLiteral: Self.IntegerLiteralType)

Creates an instance initialized to the specified integer value.

**Required** Default implementation provided.

## Relationships

### Inherited By

- BinaryFloatingPoint
- BinaryInteger
- FixedWidthInteger
- FloatingPoint
- Numeric
- SignedInteger
- SignedNumeric
- UnsignedInteger

### Conforming Types

- Double
- Float
- Float16
- Float80
- Int
- Int128
- Int16
- Int32
- Int64
- Int8
- StaticBigInt
- UInt
- UInt128
- UInt16
- UInt32
- UInt64
- UInt8

## See Also

### Value Literals

protocol ExpressibleByFloatLiteral

A type that can be initialized with a floating-point literal.

protocol ExpressibleByBooleanLiteral

A type that can be initialized with the Boolean literals `true` and `false`.

protocol ExpressibleByNilLiteral

A type that can be initialized using the nil literal, `nil`.

struct StaticBigInt

An immutable arbitrary-precision signed integer.

