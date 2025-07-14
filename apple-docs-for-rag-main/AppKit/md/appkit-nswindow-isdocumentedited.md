

- AppKit
- NSWindow
-  isDocumentEdited 

Instance Property

# isDocumentEdited

A Boolean value that indicates whether the window’s document has been edited.

macOS

``` source
@MainActor
var isDocumentEdited: Bool { get set }
```

## Discussion

The value of this property is true when the window’s document has been edited; otherwise, false. Initially, by default, `NSWindow` objects are in the “not edited” state.

You should set isDocumentEdited to true every time the window’s document changes in such a way that it needs to be saved. Conversely, when the document is saved, you should set the property to true when the window’s document has been edited; otherwise, false. Then, before closing the window you can examine the value of the property to determine whether to allow the user a chance to save the document.

