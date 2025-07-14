

- App Intents
-  EntityURLRepresentation 

Structure

# EntityURLRepresentation

The URL representation of an app entity.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct EntityURLRepresentation where Entity : AppEntity
```

## Overview

Note that you need to use a universal link for your URL representation, you can’t use a custom URL scheme. For more information about universal links, see Allowing apps and websites to link to your content.

## Topics

### Initializers

init(String)

init(stringInterpolation: EntityURLRepresentation&lt;Entity>.StringInterpolation)

Creates an instance from a string interpolation.

init(stringLiteral: String)

Creates an instance initialized to the given string value.

### Type Aliases

typealias ExtendedGraphemeClusterLiteralType

A type that represents an extended grapheme cluster literal.

typealias StringLiteralType

A type that represents a string literal.

typealias UnicodeScalarLiteralType

A type that represents a Unicode scalar literal.

### Default Implementations

ExpressibleByExtendedGraphemeClusterLiteral Implementations

ExpressibleByStringInterpolation Implementations

ExpressibleByStringLiteral Implementations

## Relationships

### Conforms To

- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringInterpolation
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral

