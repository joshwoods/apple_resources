

- AppKit
- NSDocumentController
-  addDocument(\_:) 

Instance Method

# addDocument(\_:)

Adds the given document to the list of open documents.

macOS

``` source
@MainActor
func addDocument(_ document: NSDocument)
```

## Parameters 

`document`  

The document to add.

## Discussion

The `open...` methods automatically call addDocument(_:). This method is mostly provided for subclasses that want to know when documents arrive.

## See Also

### Managing Documents

var documents: [NSDocument]

The document objects managed by the receiver.

var currentDocument: NSDocument?

The document object associated with the main window.

func document(for: NSWindow) -> NSDocument?

Returns the document object whose window controller owns a specified window.

var hasEditedDocuments: Bool

A Boolean value indicating whether the receiver has any documents with unsaved changes.

func removeDocument(NSDocument)

Removes the given document from the list of open documents.

