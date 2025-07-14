

- PackageDescription
-  Trait 

Structure

# Trait

A struct representing a package’s trait.

SwiftPM 6.1+

``` source
struct Trait
```

## Overview

Traits can be used for expressing conditional compilation and optional dependencies.

Important

Traits must be strictly additive and enabling a trait **must not** remove API.

## Topics

### Operators

static func == (Trait, Trait) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(name: String, description: String?, enabledTraits: Set&lt;String>)

Initializes a new trait.

init(stringLiteral: StringLiteralType)

Creates an instance initialized to the given string value.

### Instance Properties

var description: String?

The trait’s description.

var enabledTraits: Set&lt;String>

A set of other traits of this package that this trait enables.

var hashValue: Int

The hash value.

var name: String

The trait’s canonical name.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias ExtendedGraphemeClusterLiteralType

A type that represents an extended grapheme cluster literal.

typealias StringLiteralType

A type that represents a string literal.

typealias UnicodeScalarLiteralType

A type that represents a Unicode scalar literal.

### Type Methods

static func `default`(enabledTraits: Set&lt;String>) -> Trait

Declares the default traits for this package.

static func trait(name: String, description: String?, enabledTraits: Set&lt;String>) -> Trait

Initializes a new trait.

### Default Implementations

Equatable Implementations

ExpressibleByExtendedGraphemeClusterLiteral Implementations

ExpressibleByStringLiteral Implementations

## Relationships

### Conforms To

- Equatable
- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral
- Hashable

