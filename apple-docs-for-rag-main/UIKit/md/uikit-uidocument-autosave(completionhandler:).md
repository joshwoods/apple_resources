

- UIKit
- UIDocument
-  autosave(completionHandler:) 

Instance Method

# autosave(completionHandler:)

Initiates automatic saving of documents with unsaved changes.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func autosave(completionHandler: ((Bool) -> Void)? = nil)
```

``` source
@MainActor
func autosave() async -> Bool
```

## Parameters 

`completionHandler`  

A block with code to execute after automatic saving concludes. The block returns no value and has one parameter:

`success`  
true if the autosaving operation succeeds, otherwise false.

The block is invoked on the calling queue.

## Discussion

UIDocument periodically invokes this method to initiate a save operation if there are unsaved changes. You shouldn’t call this method directly. Subclasses can override it if they want to do special things with autosaving. The default implementation of this method invokes the hasUnsavedChanges method and, if that returns true, it invokes the save(to:for:completionHandler:) method.

This method should only be invoked for period-based saves. You may invoke it with the `success` parameter of the completion-handler parameter set to false and return; this makes it safe to not actually save when autosave(completionHandler:) is invoked. However, if you call save(to:for:completionHandler:), saving of document data must occur.

## See Also

### Tracking changes and autosaving

var hasUnsavedChanges: Bool

A Boolean value that indicates whether the document has any unsaved changes.

func updateChangeCount(UIDocument.ChangeKind)

Updates the change counter by indicating the kind of change.

var undoManager: UndoManager!

The undo manager for the document.

func changeCountToken(for: UIDocument.SaveOperation) -> Any

Returns a change token for a specific save operation.

func updateChangeCount(withToken: Any, for: UIDocument.SaveOperation)

Updates the change count with reference to a change-count token passed in by UIKit.

