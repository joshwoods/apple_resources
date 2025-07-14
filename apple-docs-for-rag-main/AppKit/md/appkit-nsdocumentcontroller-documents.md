

- AppKit
- NSDocumentController
-  documents 

Instance Property

# documents

The document objects managed by the receiver.

macOS

``` source
@MainActor
var documents: [NSDocument] { get }
```

## Discussion

The array contains zero or more NSDocument objects.

## See Also

### Managing Documents

func addDocument(NSDocument)

Adds the given document to the list of open documents.

var currentDocument: NSDocument?

The document object associated with the main window.

func document(for: NSWindow) -> NSDocument?

Returns the document object whose window controller owns a specified window.

var hasEditedDocuments: Bool

A Boolean value indicating whether the receiver has any documents with unsaved changes.

func removeDocument(NSDocument)

Removes the given document from the list of open documents.

