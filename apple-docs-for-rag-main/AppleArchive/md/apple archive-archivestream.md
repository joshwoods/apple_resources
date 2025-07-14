

- Apple Archive
-  ArchiveStream 

Class

# ArchiveStream

An archive stream that reads from and writes to data blobs

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
class ArchiveStream
```

## Topics

### Creating an Archive Stream

init(object: _AAOptionalObjectWrapperWithFilter&lt;_AAArchiveStreamTraits>.AAType?, owned: Bool, messageProc: ArchiveHeader._EntryFilterWrapper?)

Returns a new archive stream from the specified traits and entry message processing callback.

### Writing Directory Contents

func writeDirectoryContents(archiveFrom: FilePath, path: FilePath?, keySet: ArchiveHeader.FieldKeySet, selectUsing: ArchiveHeader.EntryFilter?, flags: ArchiveFlags, threadCount: Int) throws

Writes all entries from a directory to the archive stream.

### Extracting Data

static func extractStream(extractingTo: FilePath, selectUsing: ArchiveHeader.EntryFilter?, flags: ArchiveFlags, threadCount: Int) -> ArchiveStream?

Opens an extract output archive stream.

static func withExtractStream&lt;E>(extractingTo: FilePath, selectUsing: ArchiveHeader.EntryFilter?, flags: ArchiveFlags, threadCount: Int, (ArchiveStream) throws -> E) throws -> E

Calls the given closure with an extract output archive stream.

### Encoding Data

static func encodeStream(writingTo: ArchiveByteStream, selectUsing: ArchiveHeader.EntryFilter?, flags: ArchiveFlags, threadCount: Int) -> ArchiveStream?

Opens an encode output archive stream.

static func withEncodeStream&lt;E>(writingTo: ArchiveByteStream, selectUsing: ArchiveHeader.EntryFilter?, flags: ArchiveFlags, threadCount: Int, (ArchiveStream) throws -> E) throws -> E

Calls the given closure with an encode output archive stream.

### Decoding Data

static func decodeStream(readingFrom: ArchiveByteStream, selectUsing: ArchiveHeader.EntryFilter?, flags: ArchiveFlags, threadCount: Int) -> ArchiveStream?

Opens a decode input archive stream.

static func withDecodeStream&lt;E>(readingFrom: ArchiveByteStream, selectUsing: ArchiveHeader.EntryFilter?, flags: ArchiveFlags, threadCount: Int, (ArchiveStream) throws -> E) throws -> E

Calls the given closure with a decode input archive stream.

### Converting Data

static func convertStream(writingTo: ArchiveStream, insertKeySet: ArchiveHeader.FieldKeySet, removeKeySet: ArchiveHeader.FieldKeySet, selectUsing: ArchiveHeader.EntryFilter?, flags: ArchiveFlags, threadCount: Int) -> ArchiveStream?

Opens a convert output archive stream.

static func withConvertStream&lt;E>(writingTo: ArchiveStream, insertKeySet: ArchiveHeader.FieldKeySet, removeKeySet: ArchiveHeader.FieldKeySet, selectUsing: ArchiveHeader.EntryFilter?, flags: ArchiveFlags, threadCount: Int, (ArchiveStream) throws -> E) throws -> E

Calls the given closure with a convert output archive stream.

### Processing Data

static func process(readingFrom: ArchiveStream, writingTo: ArchiveStream, selectUsing: ArchiveHeader.EntryFilter?, flags: ArchiveFlags, threadCount: Int) throws -> Int

Processes archive elements between two archive streams.

### Using Custom Streams

static func customStream&lt;C>(instance: C) -> ArchiveStream?

Returns a new archive stream instance mapped to an object that conforms to the archive stream protocol.

static func withStream&lt;C, E>(wrapping: C, (ArchiveStream) throws -> E) throws -> E

Calls the given closure with an archive stream instance mapped to an object that conforms to the archive stream protocol.

## Relationships

### Conforms To

- ArchiveStreamProtocol

## See Also

### Apple Archive streams

protocol ArchiveStreamProtocol

A set of methods that defines the interface for using an archive stream that reads from and writes to data blobs.

protocol ArchiveByteStreamProtocol

A set of methods that defines the interface for using an archive stream that reads from and writes to buffers.

class ArchiveByteStream

An archive stream that reads from and writes to buffers.

