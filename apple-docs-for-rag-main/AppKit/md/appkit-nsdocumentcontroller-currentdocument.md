

- AppKit
- NSDocumentController
-  currentDocument 

Instance Property

# currentDocument

The document object associated with the main window.

macOS

``` source
@MainActor
var currentDocument: NSDocument? { get }
```

## Discussion

The value of this property is `nil` if it is called when the app is not active. This can occur during processing of a drag-and-drop operation, for example, in an implementation of `readSelectionFromPasteboard:`. In such a case, send the following message instead from an `NSView` subclass associated with the document:

```
[[[self window] windowController] document];
```

## See Also

### Managing Documents

var documents: [NSDocument]

The document objects managed by the receiver.

func addDocument(NSDocument)

Adds the given document to the list of open documents.

func document(for: NSWindow) -> NSDocument?

Returns the document object whose window controller owns a specified window.

var hasEditedDocuments: Bool

A Boolean value indicating whether the receiver has any documents with unsaved changes.

func removeDocument(NSDocument)

Removes the given document from the list of open documents.

