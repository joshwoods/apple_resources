

- AppKit
- NSDocument
-  isEntireFileLoaded 

Instance Property

# isEntireFileLoaded

A Boolean value that indicates whether the document’s file is completely loaded into memory.

macOS 10.7+

``` source
nonisolated
var isEntireFileLoaded: Bool { get }
```

## Return Value

true if the document’s entire file is loaded into memory; otherwise false.

## Discussion

The default value of this property is true, which signifies that the entire file is loaded into memory. You can override this property to return false if additional data needs to be read from the file. `NSDocument` may use this value to do things like prevent volume ejection or warn the user when a partially loaded file disappears from the file system.

## See Also

### Getting Document Metadata

var fileURL: URL?

The location of the document’s on-disk representation.

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

var isInViewingMode: Bool

A Boolean value that indicates whether the document is in read-only mode.

