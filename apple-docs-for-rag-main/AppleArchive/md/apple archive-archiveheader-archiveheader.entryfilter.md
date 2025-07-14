

- Apple Archive
- ArchiveHeader
-  ArchiveHeader.EntryFilter 

Type Alias

# ArchiveHeader.EntryFilter

A type alias for the parameters passed to an archive stream operation’s entry selection and status closure.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
typealias EntryFilter = (ArchiveHeader.EntryMessage, FilePath, ArchiveHeader.EntryFilterData?) -> ArchiveHeader.EntryMessageStatus
```

## See Also

### Manipulating Entries

class EntryAttributes

An object that describes archive entry attributes.

class EntryXATBlob

An object that describes the extended attributes of an archive entry.

var entryType: ArchiveHeader.EntryType?

The entry type from `TYP` field, or `nil` if missing or invalid.

struct EntryType

Constants that specify the filesystem entry types.

struct EntryMessage

Constants that represent message values for the entry message filters.

enum EntryFilterData

Enumerations that represent entry filter data.

struct EntryMessageStatus

Statuses that you return from an archive stream operation’s entry selection and status closure.

