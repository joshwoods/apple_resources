

- MusicKit
-  MusicItemCollection 

Structure

# MusicItemCollection

A collection of music items.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct MusicItemCollection where MusicItemType : MusicItem
```

## Topics

### Operators

static func += (inout MusicItemCollection&lt;MusicItemType>, MusicItemCollection&lt;MusicItemType>)

Appends contents of a collection representing a next batch, in the right hand side, to the existing collection on the left hand side.

### Initializers

init&lt;S>(S)

### Instance Properties

var hasNextBatch: Bool

A Boolean value that indicates whether the collection has information that allows it to fetch a subsequent batch of items.

var title: String?

An optional title for the collection.

### Instance Methods

func nextBatch(limit: Int?) async throws -> MusicItemCollection&lt;MusicItemType>?

Fetches the next batch of items asynchronously.

func nextBatch(limit: Int?) async throws -> MusicItemCollection&lt;MusicItemType>?

Fetches the next batch of items asynchronously.

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

CustomDebugStringConvertible Implementations

CustomStringConvertible Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

ExpressibleByArrayLiteral Implementations

Hashable Implementations

RandomAccessCollection Implementations

Sequence Implementations

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- ExpressibleByArrayLiteral
- Hashable
- RandomAccessCollection
- Sendable
- Sequence

## See Also

### Utility

protocol MusicItem

A protocol with basic requirements for music items.

struct MusicItemID

An object that represents a unique identifier for a music item.

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

