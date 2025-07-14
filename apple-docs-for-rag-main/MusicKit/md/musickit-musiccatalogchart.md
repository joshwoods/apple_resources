

- MusicKit
-  MusicCatalogChart 

Structure

# MusicCatalogChart

An object that contains popular items in the Apple Music catalog.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct MusicCatalogChart where MusicItemType : MusicCatalogChartRequestable
```

## Topics

### Instance Properties

let id: String

The unique identifier for the catalog chart.

let items: MusicItemCollection&lt;MusicItemType>

The items for the catalog chart.

let kind: MusicCatalogChartKind

The kind of catalog chart.

let title: String

The title for the catalog chart.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomStringConvertible Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Identifiable
- Sendable

