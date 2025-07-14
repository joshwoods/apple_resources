

- MusicKit
-  MusicCatalogChartKind 

Enumeration

# MusicCatalogChartKind

The available kinds of catalog charts.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum MusicCatalogChartKind
```

## Topics

### Operators

static func == (MusicCatalogChartKind, MusicCatalogChartKind) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case cityTop

case dailyGlobalTop

case mostPlayed

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias AllCases

A type that can represent a collection of all values of this type.

### Type Properties

static var allCases: [MusicCatalogChartKind]

A collection of all values of this type.

### Default Implementations

CustomStringConvertible Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

## Relationships

### Conforms To

- CaseIterable
- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

