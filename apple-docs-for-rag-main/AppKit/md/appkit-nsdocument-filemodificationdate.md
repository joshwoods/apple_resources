

- AppKit
- NSDocument
-  fileModificationDate 

Instance Property

# fileModificationDate

The last-known modification date of the document’s on-disk representation.

macOS

``` source
nonisolated
var fileModificationDate: Date? { get set }
```

## Discussion

The `NSDocument` default file saving machinery uses this information to warn the user when the on-disk representation of an open document has been modified by something other than the current app.

## See Also

### Getting Document Metadata

var fileURL: URL?

The location of the document’s on-disk representation.

var isEntireFileLoaded: Bool

A Boolean value that indicates whether the document’s file is completely loaded into memory.

var keepBackupFile: Bool

A Boolean value that indicates whether the document archives previously saved versions of the document.

var isDraft: Bool

A Boolean value that indicates whether the document is a draft that the user has not yet saved.

var fileType: String?

The name of the document type, as specified in the app’s information property-list file.

var isDocumentEdited: Bool

A Boolean value that indicates whether the document has unsaved changes.

var isInViewingMode: Bool

A Boolean value that indicates whether the document is in read-only mode.

