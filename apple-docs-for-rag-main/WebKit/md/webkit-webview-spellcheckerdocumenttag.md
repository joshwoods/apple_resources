

- WebKit
- WebView
-  spellCheckerDocumentTag 

Instance Property

# spellCheckerDocumentTag

The spell-checker document tag for this document.

macOS

``` source
@MainActor
var spellCheckerDocumentTag: Int { get }
```

## Discussion

A tag identifying the receiver’s text as a document for the spell-checker server. See the NSSpellChecker and NSSpellServer class specifications for more information on how this tag is used.

## See Also

### Related Documentation

@MainActor var spellCheckerDocumentTag: Int { get }

A tag identifying the text view’s text as a document for the spell checker server.

### Getting and Setting Document Editing Attributes

var isEditable: Bool

A Boolean that indicates whether the user is allowed to edit the document.

var smartInsertDeleteEnabled: Bool

A Boolean that indicates whether smart-space insertion and deletion is enabled.

var isContinuousSpellCheckingEnabled: Bool

A Boolean that indicates whether the web view has continuous spell-checking enabled.

var undoManager: UndoManager!

The receiver’s undo manager.

var editingDelegate: (any WebEditingDelegate)!

The receiver’s editing delegate.

func editableDOMRange(for: NSPoint) -> DOMRange!

Returns the editable DOM object located at a given point.

