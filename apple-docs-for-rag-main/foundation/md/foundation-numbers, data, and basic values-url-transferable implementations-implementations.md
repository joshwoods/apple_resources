

- Foundation
- Numbers, Data, and Basic Values
- URL
-  Transferable Implementations 

API Collection

# Transferable Implementations

## Topics

### Initializers

init(importing: URL, contentType: UTType?) async throws

Using the type’s `Transferable` conformance implementation, instantiates a value from the given file.

init(importing: Data, contentType: UTType?) async throws

Using the type’s `Transferable` conformance implementation, instantiates a value from given data.

### Instance Properties

var suggestedFilename: String?

A suggested filename of a `Transferable` value.

### Instance Methods

func export(to: URL, contentType: UTType?) async throws -> URL

Using the type’s `Transferable` conformance implementation, exports a value by writing it to a provided destination directory.

func exported(as: UTType?) async throws -> Data

Using the type’s `Transferable` conformance implementation, exports a value as binary data.

func exportedContentTypes(TransferRepresentationVisibility) -> [UTType]

Content types supported by a given value’s `Transferable` conformance for export (like drag or copy).

func importedContentTypes() -> [UTType]

Content types supported by a given value’s `Transferable` conformance for import (like drop or paste).

func withExportedFile&lt;Result>(contentType: UTType?, fileHandler: (URL) async throws -> Result) async throws -> Result

Using the type’s `Transferable` conformance implementation, exports a value by writing it to disk and removes when not needed.

### Type Aliases

typealias Representation

The data type for conformance with the Core Transferable framework.

### Type Properties

static var transferRepresentation: some TransferRepresentation

The representation for importing and exporting an item using Core Transferable.

### Type Methods

static func exportedContentTypes(visibility: TransferRepresentationVisibility) -> [UTType]

The types that the instance of a `Transferable` is able to provide a representation for.

