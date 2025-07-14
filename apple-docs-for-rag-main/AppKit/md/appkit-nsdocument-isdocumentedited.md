

- AppKit
- NSDocument
-  isDocumentEdited 

Instance Property

# isDocumentEdited

A Boolean value that indicates whether the document has unsaved changes.

macOS

``` source
@MainActor
var isDocumentEdited: Bool { get }
```

## Discussion

The value of this property is true if the document has been edited. The edited status of each document window reflects the document’s edited status.

## See Also

### Related Documentation

func updateChangeCount(NSDocument.ChangeType)

Updates the receiver’s change count according to the given change type.

var isDocumentEdited: Bool

A Boolean value that indicates whether the window’s document has been edited.

### Getting Document Metadata

var fileURL: URL?

The location of the document’s on-disk representation.

var isEntireFileLoaded: Bool

A Boolean value that indicates whether the document’s file is completely loaded into memory.

var fileModificationDate: Date?

The last-known modification date of the document’s on-disk representation.

var keepBackupFile: Bool

A Boolean value that indicates whether the document archives previously saved versions of the document.

var isDraft: Bool

A Boolean value that indicates whether the document is a draft that the user has not yet saved.

var fileType: String?

The name of the document type, as specified in the app’s information property-list file.

var isInViewingMode: Bool

A Boolean value that indicates whether the document is in read-only mode.

