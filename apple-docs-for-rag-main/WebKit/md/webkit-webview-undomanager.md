

- WebKit
- WebView
-  undoManager 

Instance Property

# undoManager

The receiver’s undo manager.

macOS

``` source
@MainActor
var undoManager: UndoManager! { get }
```

## See Also

### Getting and Setting Document Editing Attributes

var isEditable: Bool

A Boolean that indicates whether the user is allowed to edit the document.

var smartInsertDeleteEnabled: Bool

A Boolean that indicates whether smart-space insertion and deletion is enabled.

var isContinuousSpellCheckingEnabled: Bool

A Boolean that indicates whether the web view has continuous spell-checking enabled.

var spellCheckerDocumentTag: Int

The spell-checker document tag for this document.

var editingDelegate: (any WebEditingDelegate)!

The receiver’s editing delegate.

func editableDOMRange(for: NSPoint) -> DOMRange!

Returns the editable DOM object located at a given point.

