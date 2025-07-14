

- Apple Archive
- ArchiveHeader
-  ArchiveHeader.EntryMessageStatus 

Structure

# ArchiveHeader.EntryMessageStatus

Statuses that you return from an archive stream operation’s entry selection and status closure.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
struct EntryMessageStatus
```

## Topics

### Entry Message Statuses

static let cancel: ArchiveHeader.EntryMessageStatus

An entry message status that indicates the operation cancels processing as soon as possible.

static let ok: ArchiveHeader.EntryMessageStatus

An entry message status that indicates the operation keeps the entry.

static let skip: ArchiveHeader.EntryMessageStatus

An entry message status that indicates the operation skips the entry.

### Instance Properties

var description: String

A textual representation of this instance.

### Raw Values

var rawValue: Int32

init(rawValue: Int32)

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
- RawRepresentable

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

typealias EntryFilter

A type alias for the parameters passed to an archive stream operation’s entry selection and status closure.

struct EntryMessage

Constants that represent message values for the entry message filters.

enum EntryFilterData

Enumerations that represent entry filter data.

