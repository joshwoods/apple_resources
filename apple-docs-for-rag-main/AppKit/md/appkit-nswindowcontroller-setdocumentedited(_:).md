

- AppKit
- NSWindowController
-  setDocumentEdited(\_:) 

Instance Method

# setDocumentEdited(\_:)

Sets the document edited flag for the window controller.

macOS

``` source
@MainActor
func setDocumentEdited(_ dirtyFlag: Bool)
```

## Parameters 

`dirtyFlag`  

true if the document has been edited since its last save, false if it hasn’t.

## Discussion

The window controller uses this flag to control whether its associated window shows up as dirty. You should not call this method directly for window controllers with an associated document; the document calls this method on its window controllers as needed.

## See Also

### Accessing the Document

var document: AnyObject?

The document associated with the window controller.

