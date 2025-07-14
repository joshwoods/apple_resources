

- Foundation
- Locale
-  Locale.Subdivision 

Structure

# Locale.Subdivision

A type that represents a subdivision of a region, such as a state in the US or a province in Canada.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Subdivision
```

## Topics

### Creating a subdivision

init(String)

Creates a sudivision from a Unicode identifier.

static func subdivision(for: Locale.Region) -> Locale.Subdivision

Returns the subdivision representing the given region as a whole.

### Examining subdivision properties

var identifier: String

The subdivision’s Unicode identifier.

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Decodable
- Encodable
- Equatable
- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral
- Hashable
- Sendable

## See Also

### Getting region components

var region: Locale.Region?

The region used by the locale.

struct Region

A type that represents a geographic region, for use in specifying a locale or language.

var subdivision: Locale.Subdivision?

The optional subdivision of the region used by this locale.

var variant: Locale.Variant?

An optional variant used by the locale.

struct Variant

A type that represents a locale’s languate variant.

