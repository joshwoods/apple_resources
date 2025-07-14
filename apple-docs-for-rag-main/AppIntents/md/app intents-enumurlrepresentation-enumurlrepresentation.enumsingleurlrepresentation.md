

- App Intents
- EnumURLRepresentation
-  EnumURLRepresentation.EnumSingleURLRepresentation 

Structure

# EnumURLRepresentation.EnumSingleURLRepresentation

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct EnumSingleURLRepresentation
```

Available when `Enum` conforms to `AppEnum`.

## Topics

### Initializers

init(stringInterpolation: EnumURLRepresentation&lt;Enum>.StringInterpolation)

Creates an instance from a string interpolation.

init(stringLiteral: EnumURLRepresentation&lt;Enum>.StringLiteralType)

Creates an instance initialized to the given string value.

### Type Aliases

typealias ExtendedGraphemeClusterLiteralType

A type that represents an extended grapheme cluster literal.

typealias StringInterpolation

The type each segment of a string literal containing interpolations should be appended to.

typealias StringLiteralType

A type that represents a string literal.

typealias UnicodeScalarLiteralType

A type that represents a Unicode scalar literal.

### Default Implementations

ExpressibleByExtendedGraphemeClusterLiteral Implementations

ExpressibleByStringLiteral Implementations

## Relationships

### Conforms To

- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringInterpolation
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral

