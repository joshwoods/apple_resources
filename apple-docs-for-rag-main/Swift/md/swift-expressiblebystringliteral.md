

- Swift
-  ExpressibleByStringLiteral 

Protocol

# ExpressibleByStringLiteral

A type that can be initialized with a string literal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol ExpressibleByStringLiteral : ExpressibleByExtendedGraphemeClusterLiteral
```

## Overview

The `String` and `StaticString` types conform to the `ExpressibleByStringLiteral` protocol. You can initialize a variable or constant of either of these types using a string literal of any length.

```
let picnicGuest = "Deserving porcupine"
```

# Conforming to ExpressibleByStringLiteral

To add `ExpressibleByStringLiteral` conformance to your custom type, implement the required initializer.

## Topics

### Associated Types

associatedtype StringLiteralType : _ExpressibleByBuiltinStringLiteral

A type that represents a string literal.

**Required**

### Initializers

init(stringLiteral: Self.StringLiteralType)

Creates an instance initialized to the given string value.

**Required**

## Relationships

### Inherits From

- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByUnicodeScalarLiteral

### Inherited By

- ExpressibleByStringInterpolation
- StringProtocol

### Conforming Types

- StaticString
- String
- String.LocalizationValue
- Substring

## See Also

### String Literals

protocol ExpressibleByExtendedGraphemeClusterLiteral

A type that can be initialized with a string literal containing a single extended grapheme cluster.

protocol ExpressibleByUnicodeScalarLiteral

A type that can be initialized with a string literal containing a single Unicode scalar value.

protocol ExpressibleByStringInterpolation

A type that can be initialized by string interpolation with a string literal that includes expressions.

protocol StringInterpolationProtocol

Represents the contents of a string literal with interpolations while it’s being built up.

struct DefaultStringInterpolation

Represents a string literal with interpolations while it is being built up.

