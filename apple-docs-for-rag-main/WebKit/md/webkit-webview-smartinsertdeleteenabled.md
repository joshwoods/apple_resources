

- WebKit
- WebView
-  smartInsertDeleteEnabled 

Instance Property

# smartInsertDeleteEnabled

A Boolean that indicates whether smart-space insertion and deletion is enabled.

macOS

``` source
@MainActor
var smartInsertDeleteEnabled: Bool { get set }
```

## Discussion

true if the receiver inserts or deletes space around selected words so as to preserve proper spacing and punctuation. false if it inserts and deletes exactly what’s selected.

## See Also

### Getting and Setting Document Editing Attributes

var isEditable: Bool

A Boolean that indicates whether the user is allowed to edit the document.

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

