

- Swift
-  ExpressibleByBooleanLiteral 

Protocol

# ExpressibleByBooleanLiteral

A type that can be initialized with the Boolean literals `true` and `false`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol ExpressibleByBooleanLiteral
```

## Overview

`Bool`, `DarwinBoolean`, `ObjCBool`, and `WindowsBool` are treated as Boolean values. Expanding this set to include types that represent more than simple Boolean values is discouraged.

To add `ExpressibleByBooleanLiteral` conformance to your custom type, implement the `init(booleanLiteral:)` initializer that creates an instance of your type with the given Boolean value.

## Topics

### Associated Types

associatedtype BooleanLiteralType : _ExpressibleByBuiltinBooleanLiteral

A type that represents a Boolean literal, such as `Bool`.

**Required**

### Initializers

init(booleanLiteral: Self.BooleanLiteralType)

Creates an instance initialized to the given Boolean value.

**Required**

## Relationships

### Conforming Types

- Bool

## See Also

### Value Literals

protocol ExpressibleByIntegerLiteral

A type that can be initialized with an integer literal.

protocol ExpressibleByFloatLiteral

A type that can be initialized with a floating-point literal.

protocol ExpressibleByNilLiteral

A type that can be initialized using the nil literal, `nil`.

struct StaticBigInt

An immutable arbitrary-precision signed integer.

