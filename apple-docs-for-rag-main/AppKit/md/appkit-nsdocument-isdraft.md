

- AppKit
- NSDocument
-  isDraft 

Instance Property

# isDraft

A Boolean value that indicates whether the document is a draft that the user has not yet saved.

macOS 10.8+

``` source
nonisolated
var isDraft: Bool { get set }
```

## Discussion

The system presents a Save dialog when the user closes a draft document. Only documents with non-`nil` values for the fileURL property should be considered drafts.

## See Also

### Getting Document Metadata

var fileURL: URL?

The location of the document’s on-disk representation.

var isEntireFileLoaded: Bool

A Boolean value that indicates whether the document’s file is completely loaded into memory.

var fileModificationDate: Date?

The last-known modification date of the document’s on-disk representation.

var keepBackupFile: Bool

A Boolean value that indicates whether the document archives previously saved versions of the document.

var fileType: String?

The name of the document type, as specified in the app’s information property-list file.

var isDocumentEdited: Bool

A Boolean value that indicates whether the document has unsaved changes.

var isInViewingMode: Bool

A Boolean value that indicates whether the document is in read-only mode.

