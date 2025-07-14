

- Apple Archive
- ArchiveHeader
-  ArchiveHeader.EntryAttributes 

Class

# ArchiveHeader.EntryAttributes

An object that describes archive entry attributes.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
class EntryAttributes
```

## Topics

### Instance Properties

var btm: timespec?

A time specification value that represents the backup time of the entry.

var ctm: timespec?

A time specification value that represents the creation time of the entry.

var flg: UInt32?

An unsigned integer that represents the BSD flags of the entry.

var gid: UInt32?

An unsigned integer that represents the group ID of the entry.

var mod: UInt32?

An unsigned integer that represents the file modes of the entry.

var mtm: timespec?

A time specification value that represents the modification time of the entry.

var uid: UInt32?

An unsigned integer that represents the user ID of the entry.

## See Also

### Manipulating Entries

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

