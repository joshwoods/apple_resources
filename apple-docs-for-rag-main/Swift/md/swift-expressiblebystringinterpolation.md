

- Swift
-  ExpressibleByStringInterpolation 

Protocol

# ExpressibleByStringInterpolation

A type that can be initialized by string interpolation with a string literal that includes expressions.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol ExpressibleByStringInterpolation : ExpressibleByStringLiteral
```

## Overview

Use string interpolation to include one or more expressions in a string literal, wrapped in a set of parentheses and prefixed by a backslash. For example:

```
let price = 2
let number = 3
let message = "One cookie: $\(price), \(number) cookies: $\(price * number)."
print(message)
// Prints "One cookie: $2, 3 cookies: $6."
```

# Extending the Default Interpolation Behavior

Add new interpolation behavior to existing types by extending `DefaultStringInterpolation`, the type that implements interpolation for types like `String` and `Substring`, to add an overload of `appendInterpolation(_:)` with their new behavior.

For more information, see the `DefaultStringInterpolation` and `StringInterpolationProtocol` documentation.

# Creating a Type That Supports the Default String Interpolation

To create a new type that supports string literals and interpolation, but that doesn’t need any custom behavior, conform the type to `ExpressibleByStringInterpolation` and implement the `init(stringLiteral: String)` initializer declared by the `ExpressibleByStringLiteral` protocol. Swift will automatically use `DefaultStringInterpolation` as the interpolation type and provide an implementation for `init(stringInterpolation:)` that passes the interpolated literal’s contents to `init(stringLiteral:)`, so you don’t need to implement anything specific to this protocol.

# Creating a Type That Supports Custom String Interpolation

If you want a conforming type to differentiate between literal and interpolated segments, restrict the types that can be interpolated, support different interpolators from the ones on `String`, or avoid constructing a `String` containing the data, the type must specify a custom `StringInterpolation` associated type. This type must conform to `StringInterpolationProtocol` and have a matching `StringLiteralType`.

For more information, see the `StringInterpolationProtocol` documentation.

## Topics

### Associated Types

associatedtype StringInterpolation : StringInterpolationProtocol = DefaultStringInterpolation

The type each segment of a string literal containing interpolations should be appended to.

**Required**

### Initializers

init(stringInterpolation: Self.StringInterpolation)

Creates an instance from a string interpolation.

**Required** Default implementation provided.

## Relationships

### Inherits From

- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral

### Inherited By

- StringProtocol

### Conforming Types

- String
- String.LocalizationValue
- Substring

## See Also

### String Literals

protocol ExpressibleByStringLiteral

A type that can be initialized with a string literal.

protocol ExpressibleByExtendedGraphemeClusterLiteral

A type that can be initialized with a string literal containing a single extended grapheme cluster.

protocol ExpressibleByUnicodeScalarLiteral

A type that can be initialized with a string literal containing a single Unicode scalar value.

protocol StringInterpolationProtocol

Represents the contents of a string literal with interpolations while it’s being built up.

struct DefaultStringInterpolation

Represents a string literal with interpolations while it is being built up.

