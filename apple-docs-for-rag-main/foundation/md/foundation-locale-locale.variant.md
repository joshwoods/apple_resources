

- Foundation
- Locale
-  Locale.Variant 

Structure

# Locale.Variant

A type that represents a locale’s languate variant.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Variant
```

## Overview

This type corresponds to the Unicode variant subtag, such as `posix`.

## Topics

### Creating a variant

init(String)

Creates a variant from a BCP 47 identifier.

### Examining variant properties

var identifier: String

The variant’s BCP 47 identifier.

### Type Properties

static let posix: Locale.Variant

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

struct Subdivision

A type that represents a subdivision of a region, such as a state in the US or a province in Canada.

var variant: Locale.Variant?

An optional variant used by the locale.

