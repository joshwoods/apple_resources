

- WebKit
- WebView
-  isContinuousSpellCheckingEnabled 

Instance Property

# isContinuousSpellCheckingEnabled

A Boolean that indicates whether the web view has continuous spell-checking enabled.

macOS

``` source
@MainActor
var isContinuousSpellCheckingEnabled: Bool { get set }
```

## Discussion

true if the object has continuous spell-checking enabled; otherwise, false.

## See Also

### Getting and Setting Document Editing Attributes

var isEditable: Bool

A Boolean that indicates whether the user is allowed to edit the document.

var smartInsertDeleteEnabled: Bool

A Boolean that indicates whether smart-space insertion and deletion is enabled.

var spellCheckerDocumentTag: Int

The spell-checker document tag for this document.

var undoManager: UndoManager!

The receiver’s undo manager.

var editingDelegate: (any WebEditingDelegate)!

The receiver’s editing delegate.

func editableDOMRange(for: NSPoint) -> DOMRange!

Returns the editable DOM object located at a given point.

