

- MusicKit
-  MusicAttributeProperty 

Class

# MusicAttributeProperty

An identifier for a music item attribute property from a specific root type to a specific resulting value type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class MusicAttributeProperty where Value : Decodable
```

## Topics

### Instance Properties

var description: String

A textual representation of this instance.

## Relationships

### Inherits From

- PartialMusicProperty

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Utility

protocol MusicItem

A protocol with basic requirements for music items.

struct MusicItemID

An object that represents a unique identifier for a music item.

struct MusicItemCollection

A collection of music items.

protocol MusicPropertyContainer

A protocol for music items that allow loading additional properties that you can fetch asynchronously.

class MusicRelationshipProperty

An identifier for a music item relationship property from a specific root type to a specific value type for the element of the resulting collection.

class MusicExtendedAttributeProperty

An identifier for a music item extended attribute property from a specific root type to a specific resulting value type.

class PartialMusicAsyncProperty

A partially type-erased identifier for a music item property that you can fetch asynchronously from a concrete root type to any resulting value type.

class PartialMusicProperty

A partially type-erased identifier for a music item property from a concrete root type to any resulting value type.

class AnyMusicProperty

A type-erased identifier for a music item property, from any root type to any resulting value type.

