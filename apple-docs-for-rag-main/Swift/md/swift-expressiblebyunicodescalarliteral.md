

- Swift
-  ExpressibleByUnicodeScalarLiteral 

Protocol

# ExpressibleByUnicodeScalarLiteral

A type that can be initialized with a string literal containing a single Unicode scalar value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol ExpressibleByUnicodeScalarLiteral
```

## Overview

The `String`, `StaticString`, `Character`, and `Unicode.Scalar` types all conform to the `ExpressibleByUnicodeScalarLiteral` protocol. You can initialize a variable of any of these types using a string literal that holds a single Unicode scalar.

```
let ñ: Unicode.Scalar = "ñ"
print(ñ)
// Prints "ñ"
```

# Conforming to ExpressibleByUnicodeScalarLiteral

To add `ExpressibleByUnicodeScalarLiteral` conformance to your custom type, implement the required initializer.

## Topics

### Associated Types

associatedtype UnicodeScalarLiteralType : _ExpressibleByBuiltinUnicodeScalarLiteral

A type that represents a Unicode scalar literal.

**Required**

### Initializers

init(unicodeScalarLiteral: Self.UnicodeScalarLiteralType)

Creates an instance initialized to the given value.

**Required** Default implementation provided.

## Relationships

### Inherited By

- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringInterpolation
- ExpressibleByStringLiteral
- StringProtocol

### Conforming Types

- Character
- StaticString
- String
- String.LocalizationValue
- Substring
- Unicode.Scalar

## See Also

### String Literals

protocol ExpressibleByStringLiteral

A type that can be initialized with a string literal.

protocol ExpressibleByExtendedGraphemeClusterLiteral

A type that can be initialized with a string literal containing a single extended grapheme cluster.

protocol ExpressibleByStringInterpolation

A type that can be initialized by string interpolation with a string literal that includes expressions.

protocol StringInterpolationProtocol

Represents the contents of a string literal with interpolations while it’s being built up.

struct DefaultStringInterpolation

Represents a string literal with interpolations while it is being built up.

