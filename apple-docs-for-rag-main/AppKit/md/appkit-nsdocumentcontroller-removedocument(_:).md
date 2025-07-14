

- AppKit
- NSDocumentController
-  removeDocument(\_:) 

Instance Method

# removeDocument(\_:)

Removes the given document from the list of open documents.

macOS

``` source
@MainActor
func removeDocument(_ document: NSDocument)
```

## Parameters 

`document`  

The document to remove.

## Discussion

A document will automatically call removeDocument(_:) when it closes. This method is mostly provided for subclasses that want to know when documents close.

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

var hasEditedDocuments: Bool

A Boolean value indicating whether the receiver has any documents with unsaved changes.

