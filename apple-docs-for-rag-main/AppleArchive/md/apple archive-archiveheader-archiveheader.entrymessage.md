

- Apple Archive
- ArchiveHeader
-  ArchiveHeader.EntryMessage 

Structure

# ArchiveHeader.EntryMessage

Constants that represent message values for the entry message filters.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
struct EntryMessage
```

## Topics

### Entry Messages

static let convertExclude: ArchiveHeader.EntryMessage

An entry message indicating the conversion operation has skipped the entry as the path data is an archive header instance.

static let decodeReading: ArchiveHeader.EntryMessage

An entry message indicating the decoder operation is reading the entry at path.

static let encodeScanning: ArchiveHeader.EntryMessage

An entry message indicating the encoder operation is scanning the entry at path.

static let encodeWriting: ArchiveHeader.EntryMessage

An entry message indicating the encoder operation is writing the entry at path.

static let extractACL: ArchiveHeader.EntryMessage

An entry message indicating the extraction operation has modified entry access control lists.

static let extractAttributes: ArchiveHeader.EntryMessage

An entry message indicating the extraction operation has modified entry attributes, and that the data is an entry attributes instance.

static let extractBegin: ArchiveHeader.EntryMessage

An entry message indicating the extraction operation has began, this is the first message for this entry.

static let extractEnd: ArchiveHeader.EntryMessage

An entry message indicating the extraction operation has ended, this is the last message for this entry.

static let extractFail: ArchiveHeader.EntryMessage

An entry message indicating the extraction operation has failed, this is the last message for this entry.

static let extractXAT: ArchiveHeader.EntryMessage

An entry message indicating the extraction operation has modified entry extended attributes, and that the data is an entry extended attributes blob.

static let processExclude: ArchiveHeader.EntryMessage

An entry message indicating the process operation has skipped this entry and that the data is an archive header instance.

static let searchExclude: ArchiveHeader.EntryMessage

An entry message indicating the operation has excluded the entry, specified by path, in search.

static let searchFail: ArchiveHeader.EntryMessage

An entry message indicating the operation has reported an error in search.

static let searchPruneDirectory: ArchiveHeader.EntryMessage

An entry message indicating the operation has skipped the directory, specified by path, in search.

### Instance Properties

var description: String

A textual representation of this instance.

### Raw Values

var rawValue: UInt32

init(rawValue: UInt32)

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

enum EntryFilterData

Enumerations that represent entry filter data.

struct EntryMessageStatus

Statuses that you return from an archive stream operation’s entry selection and status closure.

