

- SwiftUI
-  FileDocument 

Protocol

# FileDocument

A type that you use to serialize documents to and from file.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
@preconcurrency
protocol FileDocument : Sendable
```

## Overview

To store a document as a value type — like a structure — create a type that conforms to the `FileDocument` protocol and implement the required methods and properties. Your implementation:

- Provides a list of the content types that the document can read from and write to by defining readableContentTypes. If the list of content types that the document can write to is different from those that it reads from, you can optionally also define writableContentTypes.

- Loads documents from file in the init(configuration:) initializer.

- Stores documents to file by serializing their content in the fileWrapper(configuration:) method.

Important

If you store your document as a reference type — like a class — use ReferenceFileDocument instead.

Ensure that types that conform to this protocol are `Sendable`. In particular, SwiftUI calls the protocol’s methods from different isolation domains. Don’t perform serialization and deserialization on `MainActor`.

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

### Writing a document

func fileWrapper(configuration: Self.WriteConfiguration) throws -> FileWrapper

Serializes a document snapshot to a file wrapper.

**Required**

static var writableContentTypes: [UTType]

The file types that the document supports saving or exporting to.

**Required** Default implementation provided.

typealias WriteConfiguration

The configuration for writing document contents.

## Relationships

### Inherits From

- Sendable

## See Also

### Storing document data in a structure instance

struct FileDocumentConfiguration

The properties of an open file document.

