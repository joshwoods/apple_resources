

- UIKit
- UIDocument
-  undoManager 

Instance Property

# undoManager

The undo manager for the document.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var undoManager: UndoManager! { get set }
```

## Discussion

This property holds the document’s undo manager (an UndoManager object). Accessing this property lazily creates a default undo manager if a custom undo manager hasn’t been set.

The undo manager for the document is registered as an observer of various UndoManager notifications so that it can call updateChangeCount(_:) as the user makes undoable changes to the document. When a subclass sets this property and implements registers changes with it, it doesn’t need to call updateChangeCount(_:) directly or (more rarely) override hasUnsavedChanges.

## See Also

### Tracking changes and autosaving

var hasUnsavedChanges: Bool

A Boolean value that indicates whether the document has any unsaved changes.

func updateChangeCount(UIDocument.ChangeKind)

Updates the change counter by indicating the kind of change.

func changeCountToken(for: UIDocument.SaveOperation) -> Any

Returns a change token for a specific save operation.

func updateChangeCount(withToken: Any, for: UIDocument.SaveOperation)

Updates the change count with reference to a change-count token passed in by UIKit.

func autosave(completionHandler: ((Bool) -> Void)?)

Initiates automatic saving of documents with unsaved changes.

