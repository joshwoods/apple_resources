

- AppKit
- NSDocument
-  isInViewingMode 

Instance Property

# isInViewingMode

A Boolean value that indicates whether the document is in read-only mode.

macOS 10.7+

``` source
@MainActor
var isInViewingMode: Bool { get }
```

## Discussion

The value of this property is true if the document is in read-only “viewing mode,” that is, if the document is locked. You can use this information to prevent certain kinds of user actions or changes when the user is viewing an old document revision.

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

var isDraft: Bool

A Boolean value that indicates whether the document is a draft that the user has not yet saved.

var fileType: String?

The name of the document type, as specified in the app’s information property-list file.

var isDocumentEdited: Bool

A Boolean value that indicates whether the document has unsaved changes.

