

- AppKit
- NSDocumentController
-  hasEditedDocuments 

Instance Property

# hasEditedDocuments

A Boolean value indicating whether the receiver has any documents with unsaved changes.

macOS

``` source
@MainActor
var hasEditedDocuments: Bool { get }
```

## Discussion

The value of this property is true if the document controller contains documents with unsaved changes; otherwise, the value is false.

## See Also

### Managing Documents

var documents: [NSDocument]

The document objects managed by the receiver.

func addDocument(NSDocument)

Adds the given document to the list of open documents.

var currentDocument: NSDocument?

The document object associated with the main window.

func document(for: NSWindow) -> NSDocument?

Returns the document object whose window controller owns a specified window.

func removeDocument(NSDocument)

Removes the given document from the list of open documents.

