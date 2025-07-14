

- SwiftUI
-  ReferenceFileDocument 

Protocol

# ReferenceFileDocument

A type that you use to serialize reference type documents to and from file.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
@preconcurrency
protocol ReferenceFileDocument : ObservableObject, Sendable
```

## Overview

To store a document as a reference type — like a class — create a type that conforms to the `ReferenceFileDocument` protocol and implement the required methods and properties. Your implementation:

- Provides a list of the content types that the document can read from and write to by defining readableContentTypes. If the list of content types that the document can write to is different from those that it reads from, you can optionally also define writableContentTypes.

- Loads documents from file in the init(configuration:) initializer.

- Stores documents to file by providing a snapshot of the document’s content in the snapshot(contentType:) method, and then serializing that content in the fileWrapper(snapshot:configuration:) method.

Ensure that types that conform to this protocol are `Sendable`. In particular, SwiftUI calls the protocol’s methods from different isolation domains. Don’t perform serialization and deserialization on `MainActor`.

```
final class PDFDocument: ReferenceFileDocument {
    struct Storage {
        var contents: Data
    }

    static let readableContentTypes: [UTType] = [.pdf]
    let storage: OSAllocatedUnfairLock

    required init(configuration: ReadConfiguration) throws {
       guard let data = configuration.file.regularFileContents else {
           throw CocoaError(.fileReadCorruptFile)
       }
        self.storage = .init(initialState: .init(contents: data))
    }

    func snapshot(contentType: UTType) throws -> Data {
        storage.withLock { $0.contents }
    }

    func fileWrapper(snapshot: Data, configuration: WriteConfiguration) throws -> FileWrapper {
        return FileWrapper(regularFileWithContents: snapshot)
    }
}
```

Important

If you store your document as a value type — like a structure — use FileDocument instead.

## Topics

### Reading a document

init(configuration: Self.ReadConfiguration) throws

Creates a document and initializes it with the contents of a file.

**Required**

static var readableContentTypes: [UTType]

The file and data types that the document reads from.

**Required**

typealias ReadConfiguration

The configuration for reading document contents.

### Getting a snapshot

func snapshot(contentType: UTType) throws -> Self.Snapshot

Creates a snapshot that represents the current state of the document.

**Required**

associatedtype Snapshot

A type that represents the document’s stored content.

**Required**

### Writing a document

func fileWrapper(snapshot: Self.Snapshot, configuration: Self.WriteConfiguration) throws -> FileWrapper

Serializes a document snapshot to a file wrapper.

**Required**

static var writableContentTypes: [UTType]

The file types that the document supports saving or exporting to.

**Required** Default implementation provided.

typealias WriteConfiguration

The configuration for writing document contents.

## Relationships

### Inherits From

- ObservableObject
- Sendable

## See Also

### Storing document data in a class instance

struct ReferenceFileDocumentConfiguration

The properties of an open reference file document.

var undoManager: UndoManager?

The undo manager used to register a view’s undo operations.

