

- PackageDescription
-  LanguageTag 

Structure

# LanguageTag

A wrapper around an IETF language tag.

``` source
struct LanguageTag
```

## Overview

To learn more about the IETF worldwide standard for language tags, see RFC5646.

## Topics

### Creating a Language Tag

init(extendedGraphemeClusterLiteral: String)

Creates an instance initialized to the given value.

init(stringLiteral: String)

Creates an instance initialized to the given value.

init(unicodeScalarLiteral: String)

Creates an instance initialized to the given value.

init?(rawValue: String)

Creates a new instance with the specified raw value.

var rawValue: String

The corresponding value of the raw type.

### Describing a Language Tag

var description: String

A textual representation of the language tag.

### Hashing

func hash(into: inout Hasher)

Hashes the language tag by feeding the item into the given hasher.

var hashValue: Int

The hash value for language tag.

### Operator Functions

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Identifying Related Types

typealias ExtendedGraphemeClusterLiteralType

A type that represents an extended grapheme cluster literal.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

typealias StringLiteralType

A type that represents a string literal.

typealias UnicodeScalarLiteralType

A type that represents a Unicode scalar literal.

### Default Implementations

CustomStringConvertible Implementations

Equatable Implementations

ExpressibleByExtendedGraphemeClusterLiteral Implementations

ExpressibleByStringLiteral Implementations

ExpressibleByUnicodeScalarLiteral Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral
- Hashable
- RawRepresentable

## See Also

### Localizing Package Resources

var defaultLocalization: LanguageTag?

The default localization for resources.

