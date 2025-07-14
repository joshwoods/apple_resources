

- Apple Archive
- ArchiveHeader
-  field(forKey:) 

Instance Method

# field(forKey:)

Returns the field for a specified key.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
func field(forKey key: ArchiveHeader.FieldKey) -> ArchiveHeader.Field?
```

## Parameters 

`key`  

The key that the function looks up in the header.

## Return Value

The field that matches the specified key, or `nil` if the key was not found.

## See Also

### Manipulating Fields

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

class FieldKeySet

An object that represents a field key set.

