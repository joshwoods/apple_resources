

- Swift
-  ExpressibleByExtendedGraphemeClusterLiteral 

Protocol

# ExpressibleByExtendedGraphemeClusterLiteral

A type that can be initialized with a string literal containing a single extended grapheme cluster.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol ExpressibleByExtendedGraphemeClusterLiteral : ExpressibleByUnicodeScalarLiteral
```

## Overview

An *extended grapheme cluster* is a group of one or more Unicode scalar values that approximates a single user-perceived character. Many individual characters, such as “é”, “김”, and “🇮🇳”, can be made up of multiple Unicode scalar values. These code points are combined by Unicode’s boundary algorithms into extended grapheme clusters.

The `String`, `StaticString`, and `Character` types conform to the `ExpressibleByExtendedGraphemeClusterLiteral` protocol. You can initialize a variable or constant of any of these types using a string literal that holds a single character.

```
let snowflake: Character = "❄︎"
print(snowflake)
// Prints "❄︎"
```

# Conforming to ExpressibleByExtendedGraphemeClusterLiteral

To add `ExpressibleByExtendedGraphemeClusterLiteral` conformance to your custom type, implement the required initializer.

## Topics

### Associated Types

associatedtype ExtendedGraphemeClusterLiteralType : _ExpressibleByBuiltinExtendedGraphemeClusterLiteral

A type that represents an extended grapheme cluster literal.

**Required**

### Initializers

init(extendedGraphemeClusterLiteral: Self.ExtendedGraphemeClusterLiteralType)

Creates an instance initialized to the given value.

**Required** Default implementation provided.

## Relationships

### Inherits From

- ExpressibleByUnicodeScalarLiteral

### Inherited By

- ExpressibleByStringInterpolation
- ExpressibleByStringLiteral
- StringProtocol

### Conforming Types

- Character
- StaticString
- String
- String.LocalizationValue
- Substring

## See Also

### String Literals

protocol ExpressibleByStringLiteral

A type that can be initialized with a string literal.

protocol ExpressibleByUnicodeScalarLiteral

A type that can be initialized with a string literal containing a single Unicode scalar value.

protocol ExpressibleByStringInterpolation

A type that can be initialized by string interpolation with a string literal that includes expressions.

protocol StringInterpolationProtocol

Represents the contents of a string literal with interpolations while it’s being built up.

struct DefaultStringInterpolation

Represents a string literal with interpolations while it is being built up.

