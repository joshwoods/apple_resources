

- UIKit
- UIDocument
-  hasUnsavedChanges 

Instance Property

# hasUnsavedChanges

A Boolean value that indicates whether the document has any unsaved changes.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var hasUnsavedChanges: Bool { get }
```

## Return Value

true if the document has unsaved changes, otherwise false.

## Discussion

The default implementation of autosave(completionHandler:) initiates a save if this property returns true. Typical subclasses don’t need to override hasUnsavedChanges. To implement change tracking, they should instead use an UndoManager object (assigned to undoManager) to register changes or call updateChangeCount(_:) every time the user makes a change; UIKit then automatically determines whether there are unsaved changes.

## See Also

### Tracking changes and autosaving

func updateChangeCount(UIDocument.ChangeKind)

Updates the change counter by indicating the kind of change.

var undoManager: UndoManager!

The undo manager for the document.

func changeCountToken(for: UIDocument.SaveOperation) -> Any

Returns a change token for a specific save operation.

func updateChangeCount(withToken: Any, for: UIDocument.SaveOperation)

Updates the change count with reference to a change-count token passed in by UIKit.

func autosave(completionHandler: ((Bool) -> Void)?)

Initiates automatic saving of documents with unsaved changes.

