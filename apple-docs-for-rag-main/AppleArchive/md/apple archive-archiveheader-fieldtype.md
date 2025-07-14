

- Apple Archive
- ArchiveHeader
-  fieldType 

Instance Property

# fieldType

The field types of the archive header.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
var fieldType: ArchiveHeader._FieldTypes { get }
```

## See Also

### Manipulating Fields

func field(forKey: ArchiveHeader.FieldKey) -> ArchiveHeader.Field?

Returns the field for a specified key.

struct FieldKey

A type that’s an alias for the field key structure.

enum Field

An enumeration that describes the type, key, and value of a header field.

struct FieldType

Constants that specify the field type of an archive header.

var fieldKey: ArchiveHeader._FieldKeys

The field keys of the archive header.

class FieldKeySet

An object that represents a field key set.

