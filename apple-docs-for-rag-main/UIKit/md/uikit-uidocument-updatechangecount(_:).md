

- UIKit
- UIDocument
-  updateChangeCount(\_:) 

Instance Method

# updateChangeCount(\_:)

Updates the change counter by indicating the kind of change.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func updateChangeCount(_ change: UIDocument.ChangeKind)
```

## Parameters 

`change`  

A constant that indicates whether a change has been made, cleared, undone, or redone. See UIDocument.ChangeKind for more information.

## Discussion

Calling this method can affect the value returned by hasUnsavedChanges. You shouldn’t need to call method this if you access an UndoManager object from the undoManager property (or assign a custom one to it) and register changes with the undo manager.

## See Also

### Tracking changes and autosaving

var hasUnsavedChanges: Bool

A Boolean value that indicates whether the document has any unsaved changes.

var undoManager: UndoManager!

The undo manager for the document.

func changeCountToken(for: UIDocument.SaveOperation) -> Any

Returns a change token for a specific save operation.

func updateChangeCount(withToken: Any, for: UIDocument.SaveOperation)

Updates the change count with reference to a change-count token passed in by UIKit.

func autosave(completionHandler: ((Bool) -> Void)?)

Initiates automatic saving of documents with unsaved changes.

