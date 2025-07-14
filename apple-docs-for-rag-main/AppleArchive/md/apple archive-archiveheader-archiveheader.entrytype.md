

- Apple Archive
- ArchiveHeader
-  ArchiveHeader.EntryType 

Structure

# ArchiveHeader.EntryType

Constants that specify the filesystem entry types.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
struct EntryType
```

## Topics

### Entry Types

static let blockSpecial: ArchiveHeader.EntryType

A constant that indicates the entry is a block device.

static let characterSpecial: ArchiveHeader.EntryType

A constant that indicates the entry is a character device.

static let directory: ArchiveHeader.EntryType

A constant that indicates the entry is a directory.

static let door: ArchiveHeader.EntryType

A constant that indicates the entry is a door.

static let fifo: ArchiveHeader.EntryType

A constant that indicates the entry is a FIFO special file.

static let link: ArchiveHeader.EntryType

A constant that indicates the entry is a symbolic link.

static let metadata: ArchiveHeader.EntryType

A constant that indicates the entry is metadata.

static let port: ArchiveHeader.EntryType

A constant that indicates the entry is a port.

static let regularFile: ArchiveHeader.EntryType

A constant that indicates the entry is a regular file.

static let socket: ArchiveHeader.EntryType

A constant that indicates the entry is a socket.

static let whiteout: ArchiveHeader.EntryType

A constant that indicates the entry is a whiteout.

### Instance Properties

var description: String

A textual representation of this instance.

### Raw Values

init(rawValue: UInt32)

var rawValue: UInt32

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

typealias EntryFilter

A type alias for the parameters passed to an archive stream operation’s entry selection and status closure.

struct EntryMessage

Constants that represent message values for the entry message filters.

enum EntryFilterData

Enumerations that represent entry filter data.

struct EntryMessageStatus

Statuses that you return from an archive stream operation’s entry selection and status closure.

