

- AppKit
- NSDocumentController
-  document(for:) 

Instance Method

# document(for:)

Returns the document object whose window controller owns a specified window.

macOS

``` source
@MainActor
func document(for window: NSWindow) -> NSDocument?
```

## Parameters 

`window`  

The window owned by the window controller.

## Return Value

The document object whose window controller owns `window`. Returns `nil` if `window` is `nil`, if `window` has no window controller, or if the window controller does not have an association with an instance of `NSDocument`.

## See Also

### Managing Documents

var documents: [NSDocument]

The document objects managed by the receiver.

func addDocument(NSDocument)

Adds the given document to the list of open documents.

var currentDocument: NSDocument?

The document object associated with the main window.

var hasEditedDocuments: Bool

A Boolean value indicating whether the receiver has any documents with unsaved changes.

func removeDocument(NSDocument)

Removes the given document from the list of open documents.

