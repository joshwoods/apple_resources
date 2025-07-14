

- Apple Archive
- ArchiveHeader
- ArchiveHeader.EntryMessage
-  extractACL 

Type Property

# extractACL

An entry message indicating the extraction operation has modified entry access control lists.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static let extractACL: ArchiveHeader.EntryMessage
```

## See Also

### Entry Messages

static let convertExclude: ArchiveHeader.EntryMessage

An entry message indicating the conversion operation has skipped the entry as the path data is an archive header instance.

static let decodeReading: ArchiveHeader.EntryMessage

An entry message indicating the decoder operation is reading the entry at path.

static let encodeScanning: ArchiveHeader.EntryMessage

An entry message indicating the encoder operation is scanning the entry at path.

static let encodeWriting: ArchiveHeader.EntryMessage

An entry message indicating the encoder operation is writing the entry at path.

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

