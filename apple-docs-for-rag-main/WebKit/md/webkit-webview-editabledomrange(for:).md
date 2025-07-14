

- WebKit
- WebView
-  editableDOMRange(for:) 

Instance Method

# editableDOMRange(for:)

Returns the editable DOM object located at a given point.

macOS

``` source
@MainActor
func editableDOMRange(for point: NSPoint) -> DOMRange!
```

## Parameters 

`point`  

The location of the editable DOM object.

## Return Value

A single range object of the editable DOM object located at `point` in the receiver’s coordinates.

## See Also

### Related Documentation

func setSelectedDOMRange(DOMRange!, affinity: NSSelectionAffinity)

Selects a range of nodes.

var selectedDOMRange: DOMRange!

The range of the current selection.

### Getting and Setting Document Editing Attributes

var isEditable: Bool

A Boolean that indicates whether the user is allowed to edit the document.

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

