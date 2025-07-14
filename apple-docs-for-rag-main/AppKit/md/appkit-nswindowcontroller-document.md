

- AppKit
- NSWindowController
-  document 

Instance Property

# document

The document associated with the window controller.

macOS

``` source
@MainActor
unowned(unsafe) var document: AnyObject? { get set }
```

## Discussion

The value of this property is `nil` if no document is associated with the window. When a window controller is added to a document’s list of window controllers, the document uses this property to set the window controller’s document; you should not set this property. AppKit uses this property to access the document for relevant next-responder messages.

## See Also

### Accessing the Document

func setDocumentEdited(Bool)

Sets the document edited flag for the window controller.

