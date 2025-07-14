

- AppKit
- NSDocument
-  keepBackupFile 

Instance Property

# keepBackupFile

A Boolean value that indicates whether the document archives previously saved versions of the document.

macOS

``` source
nonisolated
var keepBackupFile: Bool { get }
```

## Discussion

The default value of this property is false, which causes each new save operation to replace the document’s on-disk content. If you override this method and return true, a save operation saves the document’s previous contents in a backup file before saving the current contents.

## See Also

### Getting Document Metadata

var fileURL: URL?

The location of the document’s on-disk representation.

var isEntireFileLoaded: Bool

A Boolean value that indicates whether the document’s file is completely loaded into memory.

var fileModificationDate: Date?

The last-known modification date of the document’s on-disk representation.

var isDraft: Bool

A Boolean value that indicates whether the document is a draft that the user has not yet saved.

var fileType: String?

The name of the document type, as specified in the app’s information property-list file.

var isDocumentEdited: Bool

A Boolean value that indicates whether the document has unsaved changes.

var isInViewingMode: Bool

A Boolean value that indicates whether the document is in read-only mode.

