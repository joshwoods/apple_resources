

- Foundation
- Locale
-  Locale.Collation 

Structure

# Locale.Collation

A type that represents the string sort order used by the locale.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Collation
```

## Topics

### Creating a collation

init(String)

Creates a collation from a BCP 47 identifier.

### Examining collation properties

var identifier: String

The collation’s BCP 47 identifier.

### Using special-purpose collations

static let standard: Locale.Collation

A collation that provides the default ordering for each language.

static let searchRules: Locale.Collation

A collation used for string search.

### Type Properties

static var availableCollations: [Locale.Collation]

### Type Methods

static func availableCollations(for: Locale.Language) -> [Locale.Collation]

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

### Getting ordering components

var collation: Locale.Collation

The string sort order of the locale.

