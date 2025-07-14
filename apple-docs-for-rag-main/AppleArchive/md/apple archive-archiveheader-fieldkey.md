

- Apple Archive
- ArchiveHeader
-  fieldKey 

Instance Property

# fieldKey

The field keys of the archive header.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
var fieldKey: ArchiveHeader._FieldKeys { get }
```

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

class FieldKeySet

An object that represents a field key set.

