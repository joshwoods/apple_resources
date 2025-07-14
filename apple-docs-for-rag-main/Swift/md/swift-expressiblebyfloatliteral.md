

- Swift
-  ExpressibleByFloatLiteral 

Protocol

# ExpressibleByFloatLiteral

A type that can be initialized with a floating-point literal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol ExpressibleByFloatLiteral
```

## Overview

The standard library floating-point types—`Float`, `Double`, and `Float80` where available—all conform to the `ExpressibleByFloatLiteral` protocol. You can initialize a variable or constant of any of these types by assigning a floating-point literal.

```
// Type inferred as 'Double'
let threshold = 6.0

// An array of 'Double'
let measurements = [2.2, 4.1, 3.65, 4.2, 9.1]
```

# Conforming to ExpressibleByFloatLiteral

To add `ExpressibleByFloatLiteral` conformance to your custom type, implement the required initializer.

## Topics

### Associated Types

associatedtype FloatLiteralType : _ExpressibleByBuiltinFloatLiteral

A type that represents a floating-point literal.

**Required**

### Initializers

init(floatLiteral: Self.FloatLiteralType)

Creates an instance initialized to the specified floating-point value.

**Required**

## Relationships

### Inherited By

- BinaryFloatingPoint

### Conforming Types

- Double
- Float
- Float16
- Float80

## See Also

### Value Literals

protocol ExpressibleByIntegerLiteral

A type that can be initialized with an integer literal.

protocol ExpressibleByBooleanLiteral

A type that can be initialized with the Boolean literals `true` and `false`.

protocol ExpressibleByNilLiteral

A type that can be initialized using the nil literal, `nil`.

struct StaticBigInt

An immutable arbitrary-precision signed integer.

