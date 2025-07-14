

- Apple Archive
-  ArchiveHeader 

Class

# ArchiveHeader

An AppleArchive entry header.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
class ArchiveHeader
```

## Topics

### Creating an Archive Header

init()

Creates a new empty archive header.

init?(keySet: ArchiveHeader.FieldKeySet, directory: FilePath, path: FilePath, flags: ArchiveFlags)

Creates a new archive header with fields derived from the filesystem object, at the specified directory and path.

init?(withAAEncodedData: UnsafeBufferPointer&lt;UInt8>)

Creates a new archive header from encoded data.

init(copying: ArchiveHeader)

Creates a copy of an archive header.

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

class FieldKeySet

An object that represents a field key set.

### Manipulating Entries

class EntryAttributes

An object that describes archive entry attributes.

class EntryXATBlob

An object that describes the extended attributes of an archive entry.

var entryType: ArchiveHeader.EntryType?

The entry type from `TYP` field, or `nil` if missing or invalid.

struct EntryType

Constants that specify the filesystem entry types.

typealias EntryFilter

A type alias for the parameters passed to an archive stream operation’s entry selection and status closure.

struct EntryMessage

Constants that represent message values for the entry message filters.

enum EntryFilterData

Enumerations that represent entry filter data.

struct EntryMessageStatus

Statuses that you return from an archive stream operation’s entry selection and status closure.

### Accessing File Paths

var entryPath: FilePath?

The entry from the path field, or nil if missing or invalid.

### Accessing AppleArchive Encoded Data

func withAAEncodedData&lt;R>((UnsafeBufferPointer&lt;UInt8>) throws -> R) rethrows -> R

Executes a closure with encoded data.

### Collection Requirements

func append(ArchiveHeader.Field)

func remove(at: Int) -> ArchiveHeader.Field

func removeAll()

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- Copyable
- MutableCollection
- RandomAccessCollection
- Sequence

