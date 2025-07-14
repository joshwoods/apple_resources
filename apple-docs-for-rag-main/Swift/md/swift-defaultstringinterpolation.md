

- Swift
-  DefaultStringInterpolation 

Structure

# DefaultStringInterpolation

Represents a string literal with interpolations while it is being built up.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct DefaultStringInterpolation
```

## Overview

Do not create an instance of this type directly. It is used by the compiler when you create a string using string interpolation. Instead, use string interpolation to create a new string by including values, literals, variables, or expressions enclosed in parentheses, prefixed by a backslash (`\(`…`)`).

```
let price = 2
let number = 3
let message = """
              If one cookie costs \(price) dollars, \
              \(number) cookies cost \(price * number) dollars.
              """
print(message)
// Prints "If one cookie costs 2 dollars, 3 cookies cost 6 dollars."
```

When implementing an `ExpressibleByStringInterpolation` conformance, set the `StringInterpolation` associated type to `DefaultStringInterpolation` to get the same interpolation behavior as Swift’s built-in `String` type and construct a `String` with the results. If you don’t want the default behavior or don’t want to construct a `String`, use a custom type conforming to `StringInterpolationProtocol` instead.

# Extending default string interpolation behavior

Code outside the standard library can extend string interpolation on `String` and many other common types by extending `DefaultStringInterpolation` and adding an `appendInterpolation(...)` method. For example:

```
extension DefaultStringInterpolation {
    fileprivate mutating func appendInterpolation(
             escaped value: String, asASCII forceASCII: Bool = false) {
        for char in value.unicodeScalars {
            appendInterpolation(char.escaped(asASCII: forceASCII))
        }
    }
}

print("Escaped string: \(escaped: string)")
```

See `StringInterpolationProtocol` for details on `appendInterpolation` methods.

`DefaultStringInterpolation` extensions should add only `mutating` members and should not copy `self` or capture it in an escaping closure.

## Topics

### Initializers

init(literalCapacity: Int, interpolationCount: Int)

Creates a string interpolation with storage pre-sized for a literal with the indicated attributes.

### Instance Methods

func appendInterpolation&lt;T>(T)

Interpolates the given value’s textual representation into the string literal being created.

func appendInterpolation&lt;T>(T)

Interpolates the given value’s textual representation into the string literal being created.

func appendInterpolation&lt;T>(T)

Interpolates the given value’s textual representation into the string literal being created.

func appendInterpolation&lt;T>(T)

Interpolates the given value’s textual representation into the string literal being created.

func appendInterpolation(any Any.Type)

func appendLiteral(String)

Appends a literal segment of a string interpolation.

### Type Aliases

typealias StringLiteralType

The type that should be used for literal segments.

### Default Implementations

CustomStringConvertible Implementations

TextOutputStream Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Sendable
- StringInterpolationProtocol
- TextOutputStream

## See Also

### String Literals

protocol ExpressibleByStringLiteral

A type that can be initialized with a string literal.

protocol ExpressibleByExtendedGraphemeClusterLiteral

A type that can be initialized with a string literal containing a single extended grapheme cluster.

protocol ExpressibleByUnicodeScalarLiteral

A type that can be initialized with a string literal containing a single Unicode scalar value.

protocol ExpressibleByStringInterpolation

A type that can be initialized by string interpolation with a string literal that includes expressions.

protocol StringInterpolationProtocol

Represents the contents of a string literal with interpolations while it’s being built up.

