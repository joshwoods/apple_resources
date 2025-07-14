

- WebKit
- WebView
-  isEditable 

Instance Property

# isEditable

A Boolean that indicates whether the user is allowed to edit the document.

macOS

``` source
@MainActor
var isEditable: Bool { get set }
```

## Discussion

true if the receiver allows the user to edit the HTML document, false if it doesn’t.

You can change the receiver’s document programmatically regardless of this setting.

Normally, an HTML document is not editable unless the elements within the document are editable. This property provides a low-level way to make the contents of a `WebView` object editable without altering the document or DOM structure.

## See Also

### Getting and Setting Document Editing Attributes

var smartInsertDeleteEnabled: Bool

A Boolean that indicates whether smart-space insertion and deletion is enabled.

var isContinuousSpellCheckingEnabled: Bool

A Boolean that indicates whether the web view has continuous spell-checking enabled.

var spellCheckerDocumentTag: Int

The spell-checker document tag for this document.

var undoManager: UndoManager!

The receiver’s undo manager.

var editingDelegate: (any WebEditingDelegate)!

The receiver’s editing delegate.

func editableDOMRange(for: NSPoint) -> DOMRange!

Returns the editable DOM object located at a given point.

