

- MusicKit
-  MusicItemID 

Structure

# MusicItemID

An object that represents a unique identifier for a music item.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@frozen
struct MusicItemID
```

## Topics

### Initializers

init(String)

Creates a music item identifier with a string.

init(rawValue: String)

Creates a new instance with the specified raw value.

init(stringLiteral: String)

Creates an instance initialized to the given string value.

### Instance Properties

let rawValue: String

The corresponding value of the raw type.

### Type Aliases

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

Decodable Implementations

Encodable Implementations

Equatable Implementations

ExpressibleByExtendedGraphemeClusterLiteral Implementations

ExpressibleByStringLiteral Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral
- Hashable
- MusicLibraryRequestFilterValueEquatable
- MusicLibraryRequestFilterValueMembershipComparable
- RawRepresentable
- Sendable

## See Also

### Utility

protocol MusicItem

A protocol with basic requirements for music items.

struct MusicItemCollection

A collection of music items.

protocol MusicPropertyContainer

A protocol for music items that allow loading additional properties that you can fetch asynchronously.

class MusicRelationshipProperty

An identifier for a music item relationship property from a specific root type to a specific value type for the element of the resulting collection.

class MusicExtendedAttributeProperty

An identifier for a music item extended attribute property from a specific root type to a specific resulting value type.

class MusicAttributeProperty

An identifier for a music item attribute property from a specific root type to a specific resulting value type.

class PartialMusicAsyncProperty

A partially type-erased identifier for a music item property that you can fetch asynchronously from a concrete root type to any resulting value type.

class PartialMusicProperty

A partially type-erased identifier for a music item property from a concrete root type to any resulting value type.

class AnyMusicProperty

A type-erased identifier for a music item property, from any root type to any resulting value type.

