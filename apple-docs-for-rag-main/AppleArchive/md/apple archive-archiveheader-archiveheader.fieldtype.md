

- Apple Archive
- ArchiveHeader
-  ArchiveHeader.FieldType 

Structure

# ArchiveHeader.FieldType

Constants that specify the field type of an archive header.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
struct FieldType
```

## Topics

### Field Types

static let blob: ArchiveHeader.FieldType

A constant that indicates the field is a data blob.

static let flag: ArchiveHeader.FieldType

A constant that indicates the field is a flag.

static let hash: ArchiveHeader.FieldType

A constant that indicates the field is a hash.

static let string: ArchiveHeader.FieldType

A constant that indicates the field is a string.

static let timespec: ArchiveHeader.FieldType

A constant that indicates the field is a time value.

static let uint: ArchiveHeader.FieldType

A constant that indicates the field is an unsigned integer.

### Raw Values

init(rawValue: UInt32)

var rawValue: UInt32

### Instance Properties

var description: String

A textual representation of this instance.

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
- RawRepresentable

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

var fieldKey: ArchiveHeader._FieldKeys

The field keys of the archive header.

class FieldKeySet

An object that represents a field key set.

