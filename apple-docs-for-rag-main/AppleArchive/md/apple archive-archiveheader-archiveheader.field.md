

- Apple Archive
- ArchiveHeader
-  ArchiveHeader.Field 

Enumeration

# ArchiveHeader.Field

An enumeration that describes the type, key, and value of a header field.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
enum Field
```

## Topics

### Field Constants

case blob(key: ArchiveHeader.FieldKey, size: UInt64, offset: UInt64)

An enumeration that indicates the field is a data blob.

case flag(key: ArchiveHeader.FieldKey)

An enumeration that indicates the field is a flag.

case hash(key: ArchiveHeader.FieldKey, hashFunction: ArchiveHash, value: ContiguousArray&lt;UInt8>)

An enumeration that indicates the field is a hash.

case string(key: ArchiveHeader.FieldKey, value: String)

An enumeration that indicates the field is a string.

case timespec(key: ArchiveHeader.FieldKey, value: timespec)

An enumeration that indicates the field is a time value.

case uint(key: ArchiveHeader.FieldKey, value: UInt64)

An enumeration that indicates the field is an unsigned integer.

### Instance Properties

var key: ArchiveHeader.FieldKey

The field key of this field.

var type: ArchiveHeader.FieldType

The field type of this field.

## See Also

### Manipulating Fields

func field(forKey: ArchiveHeader.FieldKey) -> ArchiveHeader.Field?

Returns the field for a specified key.

struct FieldKey

A type that’s an alias for the field key structure.

var fieldType: ArchiveHeader._FieldTypes

The field types of the archive header.

struct FieldType

Constants that specify the field type of an archive header.

var fieldKey: ArchiveHeader._FieldKeys

The field keys of the archive header.

class FieldKeySet

An object that represents a field key set.

