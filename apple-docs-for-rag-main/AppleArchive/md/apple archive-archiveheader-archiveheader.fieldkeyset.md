

- Apple Archive
- ArchiveHeader
-  ArchiveHeader.FieldKeySet 

Class

# ArchiveHeader.FieldKeySet

An object that represents a field key set.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
final class FieldKeySet
```

## Topics

### Creating a Field Key Set

init()

Creates a new empty field key set.

init?(String)

Creates a new field key set from the specified comma-separated string of three-letter keys.

init(copying: ArchiveHeader.FieldKeySet)

Creates a copy of the specified field key set.

### Specifying Default Field Key Sets

static var defaultForArchive: ArchiveHeader.FieldKeySet

A constant that contains the default key set for an archive.

static var defaultForManifest: ArchiveHeader.FieldKeySet

A constant that contains the default key set for a manifest.

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- Copyable
- CustomStringConvertible
- Equatable
- ExpressibleByArrayLiteral
- RandomAccessCollection
- Sequence
- SetAlgebra

## See Also

### Manipulating Fields

func field(forKey: ArchiveHeader.FieldKey) -> ArchiveHeader.Field?

Returns the field for a specified key.

struct FieldKey

A type that’s an alias for the field key structure.

enum Field

An enumeration that describes the type, key, and value of a header field.

var fieldType: ArchiveHeader._FieldTypes

The field types of the archive header.

struct FieldType

Constants that specify the field type of an archive header.

var fieldKey: ArchiveHeader._FieldKeys

The field keys of the archive header.

