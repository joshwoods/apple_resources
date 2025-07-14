

- Apple Archive
- ArchiveHeader
-  ArchiveHeader.EntryXATBlob 

Class

# ArchiveHeader.EntryXATBlob

An object that describes the extended attributes of an archive entry.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
class EntryXATBlob
```

## Topics

### Creating an Extended Attributes Blob

init()

Creates a new empty extended attribute blob.

init?(directory: FilePath, path: FilePath, flags: ArchiveFlags)

Creates a new extended attribute blob from the specified directory and path.

init?(withAAEncodedData: UnsafeBufferPointer&lt;UInt8>)

Creates a new archive header from encoded data.

### Applying an Extended Attributes Blob

func apply(directory: FilePath, path: FilePath, flags: ArchiveFlags) throws

Applies extended attributes to a filesystem object.

### Describing Extended Attributes

struct ExtendedAttribute

A structure that describes the extended attributes of a filesystem.

### Collection Requirements

func append(ArchiveHeader.EntryXATBlob.ExtendedAttribute)

func remove(at: Int) -> ArchiveHeader.EntryXATBlob.ExtendedAttribute

func removeAll()

func withAAEncodedData&lt;R>((UnsafeBufferPointer&lt;UInt8>) throws -> R) rethrows -> R

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- Copyable
- MutableCollection
- RandomAccessCollection
- Sequence

## See Also

### Manipulating Entries

class EntryAttributes

An object that describes archive entry attributes.

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

